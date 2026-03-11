# AI HPC Guide Collection


This is a collection of guides / code snippets for artificial intelligence (AI) workloads on high performance computing (HPC).

This is work in progress lead by the [LUMI AI Factory](lumi-ai-factory.eu) but we welcome contributions via
- opening [new issues](https://github.com/lumi-ai-factory/ai-hpc-guide-collection/issues/new)
- opening [new pull requests](https://github.com/lumi-ai-factory/ai-hpc-guide-collection/compare).


> [!IMPORTANT] 
> For most repositories, we are not the owner. We reference to them but have no control over the content of these repositories.
> Many repositories are not officially supported by the maintainers of the HPC systems.
> Please take that into account when following these guides / code snippets.

-----

## AI Container / Software environments on HPC
| Topic | What Guide | Notes |
|-------|------------|-------|
| PyTorch container | [Lumi-supercomputer/LUMI-AI-Guide (Sections 1+2)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide) | Guide for LUMI |


## Data on Lustre
| Topic | What Guide | Notes |
|-------|------------|-------|
| File Formats | [Lumi-supercomputer/LUMI-AI-Guide (Section 3)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/3-file-formats) | Guide for LUMI |
| Data Storage | [Lumi-supercomputer/LUMI-AI-Guide (Section 4)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/4-data-storage) | Guide for LUMI |

## LLM fine-tuning
| Topic | What Guide | Notes |
|-------|------------|-------|
| Huggingface Accelerate | [mimer-ai/llm_finetuning_example](github.com/mimer-ai/llm_finetuning_example) | Code snippets for Leonardo, LUMI, and Meluxina |
| Huggingface Accelerate | [CSCfi/llm-fine-tuning-examples](https://github.com/CSCfi/llm-fine-tuning-examples) | Code snippets for LUMI and Mahti |
| DeepSpeed | [AaltoRSE/llm-on-lumi/tree/main](https://github.com/AaltoRSE/llm-on-lumi/tree/main) | Code snippets for LUMI |
| Nanotron | [AaltoRSE/llm-on-lumi/tree/main](https://github.com/AaltoRSE/llm-on-lumi/tree/main) | Code snippets for LUMI |

## Multi GPU and Node Training
| Topic | What Guide | Notes |
|-------|------------|-------|
| PyTorch DDP | [Lumi-supercomputer/LUMI-AI-Guide (Section 5)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/5-multi-gpu-and-node) | Guide for LUMI |
| PyTorch DeepSpeed | [Lumi-supercomputer/LUMI-AI-Guide (Section 5)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/5-multi-gpu-and-node) | Guide for LUMI |
| Huggingface Accelerate | [CSCfi/llm-fine-tuning-examples](https://github.com/CSCfi/llm-fine-tuning-examples) | Code snippets for LUMI and Mahti |
 
## Profiling
| Topic | What Guide | Notes |
|--------|------------|-------|
| ROCm-SMI on LUMI | [Lumi-supercomputer/LUMI-AI-Guide (Section 6)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/6-monitoring-and-profiling) | Guide for LUMI |
| PyTorch Profiler | [Lumi-supercomputer/LUMI-AI-Guide (Section 6)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/6-monitoring-and-profiling) | |

## Hyperparameter optimization
| Topic | What Guide | Notes |
|--------|------------|-------|
| HPO on HPC | [AaltoRSE/hpo-on-hpc](https://github.com/AaltoRSE/hpo-on-hpc) | |

## MLOps
| Topic | What Guide | Notes |
|--------|------------|-------|
| Tensor Board | [Lumi-supercomputer/LUMI-AI-Guide (Section 7)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/7-TensorBoard-visualization) | |
| ML Flow | [docs.csc.fi/support/tutorials/ml-workflows/](https://docs.csc.fi/support/tutorials/ml-workflows/#mlflow); [Lumi-supercomputer/LUMI-AI-Guide (Section 8)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/8-MLflowlization) | Guides for LUMI and Mahti |


## Inference
| Topic | What Guide | Notes |
|--------|------------|-------|
| vLLM | [CSCfi/ai-inference-examples](https://github.com/CSCfi/ai-inference-examples) | Code snippets, not full guide |
| ollama | [CSCfi/ai-inference-examples](https://github.com/CSCfi/ai-inference-examples) | Code snippets, not full guide |

## Quantization

| Topic | What Guide | Notes |
|--------|------------|-------|
| AWQ (Activation-aware Weight Quantization)  |  [docs.csc.fi/support/tutorials/ml-llm/](https://docs.csc.fi/support/tutorials/ml-llm/#using-awq-quantization-via-llm-compressor); [CSCfi/llm-quantization-scripts](https://github.com/CSCfi/llm-quantization-scripts) | Examples for LUMI and Mahti |
| BitsandBytes  | [docs.csc.fi/support/tutorials/ml-llm/](https://docs.csc.fi/support/tutorials/ml-llm/#using-bitsandbytes-quantization); [CSCfi/llm-quantization-scripts](https://github.com/CSCfi/llm-quantization-scripts) | Examples for LUMI and Mahti |
| GPTQ (Gradient Post-training Quantization)  | [docs.csc.fi/support/tutorials/ml-llm/](https://docs.csc.fi/support/tutorials/ml-llm/#using-gptq-quantization); [CSCfi/llm-quantization-scripts](https://github.com/CSCfi/llm-quantization-scripts) | Examples for LUMI and Mahti|

## Evaluation frameworks
| Topic | What Guide | Notes |
|--------|------------|-------|
| LM Eval Harness on LUMI | [LumiOpen/lm-evaluation-harness](https://github.com/LumiOpen/lm-evaluation-harness) | Seems like a relevant fork for LUMI |


## Relevant topics where no material has been found
- Data Preprocessing on HPC
- Moving from HPC to production environments

## Relevant resources that need to be mapped
- [gitlab.tuwien.ac.at/vsc-public/training/LLMs-on-supercomputers](https://gitlab.tuwien.ac.at/vsc-public/training/LLMs-on-supercomputers)
- [amd/HPCTrainingExamples/tree/main/MLExamples](https://github.com/amd/HPCTrainingExamples/tree/main/MLExamples)
- [ENCCS/castiel-multi-gpu-ai](https://github.com/ENCCS/castiel-multi-gpu-ai)
- [openhackathons-org/End-to-End-AI-for-Science/tree/main/workspace/python](https://github.com/openhackathons-org/End-to-End-AI-for-Science/tree/main/workspace/python)
- [olcf/ai-training-series](https://github.com/olcf/ai-training-series)