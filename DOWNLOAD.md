# Download Required Habitat Datasets

Official instructions: [Habitat-Sim Dataset Guide](https://github.com/facebookresearch/habitat-sim/blob/main/DATASETS.md)

Datasets can be downloaded using the built-in Habitat-Sim utility:

```bash
python -m habitat_sim.utils.datasets_download --uids <dataset_name> --data-path data/
```

You can find the list of available dataset UIDs here:
- [datasets_download.py (official reference)](https://github.com/facebookresearch/habitat-sim/blob/main/src_python/habitat_sim/utils/datasets_download.py)
- [Hugging Face: ai-habitat](https://huggingface.co/ai-habitat)
- [Hugging Face: hssd](https://huggingface.co/hssd)


## Download Datasets Used by COOPERA

```bash
# Make sure you are in your COOPERA Habitat-Lab directory:
cd /path/to/coopera_code/habitat-lab

# xxx
python -m habitat_sim.utils.datasets_download --uids <dataset name> --data-path data/
```