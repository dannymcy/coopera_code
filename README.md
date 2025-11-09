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

## Download Habitat Datasets

See [DOWNLOAD.md](DOWNLOAD.md) for downloading required Habitat datasets.

## Human Simulation

See [HUMAN.md](HUMAN.md) for simulating humans driven by psychological traits and long-term intentions. This step is a prerequisite for running the COOPERA benchmark. You may also stop here if you are only interested in human simulation.

## COOPERA Benchmark

See [BENCHMARK.md](BENCHMARK.md) for running the COOPERA benchmark.

## Visualize Results

[Coming Soon] You may want to generate a video to visualize human-robot collaboration.

## Support

If you run into any issues, please open a new GitHub issue.

## Citation

```
@inproceedings{ma2025coopera,
  title     = {COOPERA: Continual Open-Ended Human-Robot Assistance},
  author    = {Ma, Chenyang and Lu, Kai and Desai, Ruta and Puig, Xavier and Markham, Andrew and Trigoni, Niki},
  booktitle = {Proceedings of the Conference on Neural Information Processing Systems (NeurIPS)},
  year      = {2025},
}
```

## Related Repos

We adapted some code and resources from other repos in implementation. Please check these useful repos. 
```
https://github.com/facebookresearch/habitat-lab
https://github.com/facebookresearch/habitat-sim
