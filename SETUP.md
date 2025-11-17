# Setup Instructions

> 🖥️ **Tested Environment**
> - **OS:** Ubuntu 20.04  
> - **CUDA:** 11.8  
> - **GPUs:** 3× NVIDIA A10 (24GB)  
> - **habitat-sim:** 0.3.1 (nightly)  
> - **habitat-lab:** 0.3.1 (from our fork [here](https://github.com/dannymcy/habitat-lab))

COOPERA depends on specific versions of `habitat-sim` and our forked `habitat-lab`. Please follow the steps below.

## 1. Clone the Repositories

```bash
git clone https://github.com/dannymcy/coopera_code.git
cd coopera_code
```

## 2. Clone Our Forked Habitat-Lab

```bash
git clone https://github.com/dannymcy/habitat-lab.git habitat-lab
```

After this step, your structure should look like:

```bash
coopera_code/
├── README.md
├── setup.md
├── habitat-lab/        ← our fork (0.3.1-based)
└── ...
```

## 3. Create and Activate Conda Environment

```bash
conda create -n coopera python=3.9 cmake=3.14.0
conda activate coopera
```

Or, if you prefer a path-based env, create it in the current project folder:

```bash
conda create --prefix "$(pwd)/env" python=3.9 cmake=3.14.0
conda activate "$(pwd)/env"
```

## 4. Install Habitat-Sim

```bash
conda install -c conda-forge -c aihabitat-nightly habitat-sim=0.3.1 withbullet
```

## 5. Install Our Forked Habitat-Lab

```bash
cd habitat-lab
pip install -e .
pip install -e habitat-baselines
```

This installs the ```habitat-lab``` that COOPERA modifies.

> Note: ```habitat-baselines``` may pull a ```tensorboard``` version that clashes with newer ```protobuf```. If you see a protobuf / tensorboard error run:

```bash
pip uninstall tensorboard -y
```

## 6. Install PyTorch (remember to match your CUDA version)

For CUDA 11.8 (what we used):

```bash
pip install --no-cache-dir torch==2.5.1+cu118 torchvision==0.20.1+cu118 --index-url https://download.pytorch.org/whl/cu118
```

## 7. Install Remaining Python Dependencies

```bash
pip install -r requirements.txt
```

## 8. (Optional) Fix for pytorchvideo + newer torchvision

Some environments produce:

> ModuleNotFoundError: No module named 'torchvision.transforms.functional_tensor'

This is due to a renamed import in newer ```torchvision```. To fix it, edit:

```bash
$CONDA_PREFIX/lib/python3.9/site-packages/pytorchvideo/transforms/augmentations.py
```

and change:

```bash
from torchvision.transforms import functional_tensor as F_t
```

to:

```bash
from torchvision.transforms import _functional_tensor as F_t
```

(Reference: [link](https://stackoverflow.com/questions/78955311/pytorchvideo-transforms-randaugment-import-error))