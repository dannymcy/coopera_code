# COOPERA: Continual Open-Ended Human-Robot Assistance

This is the official implementation for the NeurIPS 2025 [paper](https://arxiv.org/abs/2403.13438). For more information, please check the [project webpage](https://dannymcy.github.io/coopera/).

In this work, we introduce COOPERA, a framework for studying continual, open-ended human-robot collaboration. COOPERA includes (a) simulated humans driven by psychological traits and long-term intentions, (b) continuous human feedback, and (c) a benchmark and approach to personalize the robot's collaborative actions.

<p align="center">
  <img src="assets/teaser.jpg" width="100%">
  <br>
  <b>Continual human-robot collaboration for open-ended tasks over multiple days.</b>
</p>

<p align="center">
  <img src="assets/framework.jpg" width="100%">
  <br>
  <b>COOPERA: continual, open-ended human-robot collaboration framework.</b>
</p>

## Installation

See [SETUP.md](SETUP.md) for instructions on setting up the conda environment.

<!-- ### Prerequisites 

Prepare ```GPT API``` from [here](https://platform.openai.com/docs/api-reference/introduction) and put it in ```.../spatialpin/main/gpt_4/query.py``` line 7.

Open a public GitHub repo and put your Git token and repo name in ```.../spatialpin/main/process_3d.py``` line 476 and 477 (Github repo name is of format ```git_account_name/repo_name```).

Prepare ```One-2-3-45++ API``` for single-view object reconstruction from [here](https://www.sudo.ai/account) and put it in ```.../spatialpin/main/process_3d.py``` line 478.

Download Segment Anything backbone by running ```.../spatialpin/main/download_sam.py``` -->

### Citation

```
@inproceedings{ma2025coopera,
  title={COOPERA: Continual Open-Ended Human-Robot Assistance},
  author={Ma, Chenyang and Lu, Kai and Desai, Ruta and Puig, Xavier and Markham, Andrew and Trigoni, Niki},
  booktitle={Proceedings of the Conference on Neural Information Processing Systems (NeurIPS)},
  year={2025},
}
```

### Related Repos

We adapted some code from other repos in implementation. Please check these useful repos. 
```
https://github.com/facebookresearch/habitat-lab
https://github.com/facebookresearch/habitat-sim
