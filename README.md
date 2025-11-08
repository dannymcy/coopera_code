# COOPERA: Continual Open-Ended Human-Robot Assistance
This is the official implementation for the NeurIPS 2025 [paper](https://arxiv.org/abs/2403.13438). For more information, please check the [project webpage](https://dannymcy.github.io/coopera/).

In this work, we introduce COOPERA, a framework for studying continual, open-ended human-robot collaboration. COOPERA includes (a) simulated humans driven by psychological traits and long-term intentions, (b) continuous human feedback, and (c) a benchmark and approach to personalize the robot's collaborative actions.

<p align="center">
  <img src="assets/teaser.jpg" width="80%">
  <br>
  <b>Continual human-robot collaboration for open-ended tasks over multiple days.</b>
</p>

<p align="center">
  <img src="assets/framework.jpg" width="100%">
  <br>
  <b>COOPERA: continual, open-ended human-robot collaboration framework.</b>
</p>


<!-- ## Environment Setup
> Note: This code was developed on Ubuntu 20.04 with CUDA 11.8. The implementation of SpatialPIN depends on two seperate Github repos.

Clone the repo.
```
git clone --recurse-submodules https://github.com/dannymcy/zeroshot_task_hallucination_code.git
cd zeroshot_task_hallucination_code
```
Set up separate Python environments.
For SpatialPIN main code: 
```
cd spatialpin
conda env create -f conda_env.yaml
conda activate /your_dir/spatialpin/env
```
For LaMa image inpainting:
```
cd ..
cd lama
conda env create -f conda_env.yaml
conda activate /your_dir/lama/env
```
For both, install CUDA and PyTorch appropriate versions for your system. For example:
```
pip install --no-cache-dir torch==2.1.1+cu118 -f https://download.pytorch.org/whl/torch_stable.html
pip install --no-cache-dir torchvision --extra-index-url https://download.pytorch.org/whl/cu118
```

### Prerequisites 
Prepare ```GPT API``` from [here](https://platform.openai.com/docs/api-reference/introduction) and put it in ```.../spatialpin/main/gpt_4/query.py``` line 7.

Open a public GitHub repo and put your Git token and repo name in ```.../spatialpin/main/process_3d.py``` line 476 and 477 (Github repo name is of format ```git_account_name/repo_name```).

Prepare ```One-2-3-45++ API``` for single-view object reconstruction from [here](https://www.sudo.ai/account) and put it in ```.../spatialpin/main/process_3d.py``` line 478.

Download Segment Anything backbone by running ```.../spatialpin/main/download_sam.py``` -->