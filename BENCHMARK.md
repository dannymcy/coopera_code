# COOPERA Benchmark

🖥️ Minimum requirement: 3x GPUs with at least 24 GB VRAM each.

## Main Approach

```bash
# Remember to configure the options and set COLLABORATION_CONFIGS inside the script
CUDA_VISIBLE_DEVICES="x,y,..." python coopera_main/benchmark/main.py [OPTIONS]
```

**Options** 

**Core Configuration**
- `--collab-type[1,2]` - Collaboration type (default: 2).
- `--collab-setting[1,2,3,4]` - Collaboration setting (default: 1).
- `--use-gpt-human[True/False]` - Read human simulation results by GPT; if False, use Llama (default: True).
- `--use-gpt-robot[True/False]` - Use GPT for robot intention/task discovery; if False, use Llama (default: True).
- `--start-logic-robot[True/False]` - Restart robot intention/task discovery (default: True).
- `--start-logic-lora[True/False]` - Restart LoRA-based intention/task classification (default: True).

**GPU**
- `CUDA_VISIBLE_DEVICES="x,y"` - GPUs visible to system
- `--gpu-id n` - Single GPU ID for Habitat simulation and computing semantic similarity (default: 0)

## Baselines
```bash
# Direct Prompting
# [Coming Soon]

# Direct Finetuning
# [Coming Soon]

# Oracle
# [Coming Soon]

# Random
# [Coming Soon]

# Intention Agnostic
# [Coming Soon]

# Human & Context Agnostic
# [Coming Soon]
```