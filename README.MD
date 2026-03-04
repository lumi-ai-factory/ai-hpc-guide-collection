# AI HPC Guide Collection


This is a collection of guides / code snippets for artificial intelligence (AI) workloads on high performance computing (HPC).

This is work in progress lead by the [LUMI AI Factory](lumi-ai-factory.eu) but we welcome contributions via
- opening [new issues](https://github.com/lumi-ai-factory/ai-hpc-guide-collection/issues/new)
- opening [new pull requests](https://github.com/lumi-ai-factory/ai-hpc-guide-collection/compare).


## AI Container / Software environments on HPC
| Topic | What Guide | Notes |
|-------|------------|-------|
| PyTorch container on LUMI supercomputer | [Lumi-supercomputer/LUMI-AI-Guide (Sections 1+2)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide) | – |


## Data on Lustre
| Topic | What Guide | Notes |
|-------|------------|-------|
| File Formats | [Lumi-supercomputer/LUMI-AI-Guide (Section 3)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/3-file-formats) | |
| Data Storage | [Lumi-supercomputer/LUMI-AI-Guide (Section 4)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/4-data-storage) | |

## Multi GPU and Node Training
| Topic | What Guide | Notes |
|-------|------------|-------|
| PyTorch DDP | [Lumi-supercomputer/LUMI-AI-Guide (Section 5)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/5-multi-gpu-and-node) | |
| PyTorch DeepSpeed | [Lumi-supercomputer/LUMI-AI-Guide (Section 5)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/5-multi-gpu-and-node) | |
| Huggingface Accelerate | [CSCfi/llm-fine-tuning-examples](https://github.com/CSCfi/llm-fine-tuning-examples) | |
 
## Profiling
| Topic | What Guide | Notes |
|--------|------------|-------|
| ROCm-SMI on LUMI | [Lumi-supercomputer/LUMI-AI-Guide (Section 6)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/6-monitoring-and-profiling) | |
| PyTorch Profiler | [Lumi-supercomputer/LUMI-AI-Guide (Section 6)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/6-monitoring-and-profiling) | |

## Hyperparameter optimization
| Topic | What Guide | Notes |
|--------|------------|-------|
| HPO on HPC | [AaltoRSE/hpo-on-hpc](https://github.com/AaltoRSE/hpo-on-hpc) | |

## MLOps
| Topic | What Guide | Notes |
|--------|------------|-------|
| Tensor Board | [Lumi-supercomputer/LUMI-AI-Guide (Section 7)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/7-TensorBoard-visualization) | |
| ML Flow | [Lumi-supercomputer/LUMI-AI-Guide (Section 8)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/8-MLflowlization) | |


## Inference
| Topic | What Guide | Notes |
|--------|------------|-------|
| vLLM | [CSCfi/ai-inference-examples](https://github.com/CSCfi/ai-inference-examples) | |
| ollama | [CSCfi/ai-inference-examples](https://github.com/CSCfi/ai-inference-examples) | |

## Evaluation frameworks
| Topic | What Guide | Notes |
|--------|------------|-------|
| LM Eval Harness on LUMI | [LumiOpen/lm-evaluation-harness](https://github.com/LumiOpen/lm-evaluation-harness) | Seems like a relevant fork|


## Relevant topics where no material has been found
- Data Preprocessing on HPC
- Moving from HPC to production environments

## Relevant resources that need to be mapped
- [gitlab.tuwien.ac.at/vsc-public/training/LLMs-on-supercomputers](https://gitlab.tuwien.ac.at/vsc-public/training/LLMs-on-supercomputers)
- [mimer-ai/llm_finetuning_example](https://github.com/mimer-ai/llm_finetuning_example)
- [amd/HPCTrainingExamples/tree/main/MLExamples](https://github.com/amd/HPCTrainingExamples/tree/main/MLExamples)
- [ENCCS/castiel-multi-gpu-ai](https://github.com/ENCCS/castiel-multi-gpu-ai)
- [openhackathons-org/End-to-End-AI-for-Science/tree/main/workspace/python](https://github.com/openhackathons-org/End-to-End-AI-for-Science/tree/main/workspace/python)