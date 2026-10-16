# AI HPC Guide Collection

This is a collection of guides / code snippets for artificial intelligence (AI) workloads on high performance computing (HPC).

This is a work in progress led by the [LUMI AI Factory](https://lumi-ai-factory.eu) but we welcome contributions via
- opening [new issues](https://github.com/lumi-ai-factory/ai-hpc-guide-collection/issues/new)
- opening [new pull requests](https://github.com/lumi-ai-factory/ai-hpc-guide-collection/compare).

> [!IMPORTANT]
> For most repositories, we are not the owner. We reference to them but have no control over the content of these repositories.
> Many repositories are not officially supported by the maintainers of the HPC systems.
> Please take that into account when following these guides / code snippets.

-----

## Contents

- [Getting started / onboarding](#getting-started--onboarding)
- [AI container / software environments on HPC](#ai-container--software-environments-on-hpc)
- [Data on Lustre](#data-on-lustre)
- [Evaluation frameworks](#evaluation-frameworks)
- [Hyperparameter optimization](#hyperparameter-optimization)
- [Inference](#inference)
- [LLM fine-tuning](#llm-fine-tuning)
- [MLOps](#mlops)
- [Multi GPU and node training](#multi-gpu-and-node-training)
- [Profiling](#profiling)
- [Quantization](#quantization)
- [Relevant topics where no material has been found](#relevant-topics-where-no-material-has-been-found)
- [Relevant resources that need to be mapped](#relevant-resources-that-need-to-be-mapped)
- [HPC centre sources](#hpc-centre-sources)
- [License](#license)
- [Acknowledgements](#acknowledgements)

-----

## Getting started / onboarding

New to running AI workloads on HPC? Start here for fundamentals and hands-on introductions.

| Topic | Guide | Notes |
| --- | --- | --- |
| LUMI AI onboarding (fundamentals) | [LUMI AIF Onboarding](https://lumi-ai-factory.github.io/LUMI_AIF_Onboarding/) | Self-paced primer for newcomers for LUMI (hosted by CSC in Finland) |
| LUMI AI hands-on workshop | [Getting_Started_with_AI_workshop](https://github.com/Lumi-supercomputer/Getting_Started_with_AI_workshop) | Workshop material |
| Snellius AI onboarding | [SURF-ML/Snellius-AI-Guide](https://github.com/SURF-ML/Snellius-AI-Guide) | Fork of LUMI AI Guide for Snellius (SURF, Netherlands). |
| HPC-infrastructure foundations | [Minerva-guidebook/1 Infrastructure Foundations for Scalable LLM Training](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide1_Infrastructure_Foundations/Guide1_Infrastructure_Foundations.html) | Comprehensive infrastructure foundations guide for AI on HPC from the best practises guidebook by Minerva 4 AI. |

## AI container / software environments on HPC

Building and running container images and software environments on HPC systems.

| Topic | Guide | Notes |
| --- | --- | --- |
| PyTorch container | [Lumi-supercomputer/LUMI-AI-Guide (Sections 01+02)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide) | Guide for LUMI (hosted by CSC in Finland) |
| Running containers on LUMI | [Getting_Started_with_AI_workshop (Ch. 05)](https://github.com/Lumi-supercomputer/Getting_Started_with_AI_workshop/tree/main/05_Running_containers_on_LUMI) | Workshop material. Singularity/SingularityCE, pulling Docker images, using official LAIF containers. Container paths & course reservations are workshop-specific. |
| Building containers from conda/pip | [Getting_Started_with_AI_workshop (Ch. 06)](https://github.com/Lumi-supercomputer/Getting_Started_with_AI_workshop/tree/main/06_Bulding_containers_from_conda_pip_environments) | Workshop material. Uses `cotainr` to build containers from conda/pip environments, incl. ROCm 7.0 PyTorch on AMD GPUs. |
| Extending containers with virtual environments | [Getting_Started_with_AI_workshop (Ch. 07)](https://github.com/Lumi-supercomputer/Getting_Started_with_AI_workshop/tree/main/07_Extending_containers_with_virtual_environments_for_faster_testing) | Workshop material. Extending a container with a venv for faster iteration/testing. |
| Containers on HPC | [Minerva-guidebook/1 Infrastructure Foundations for Scalable LLM Training (1.4.9)](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide1_Infrastructure_Foundations/Guide1_Infrastructure_Foundations.html#containers-on-hpc) | A section on using containers on HPC systems from  the best practises guidebook by Minerva 4 AI. | 

## Data on Lustre

Storing and reading training data efficiently on the Lustre parallel filesystem.

| Topic | Guide | Notes |
| --- | --- | --- |
| File Formats | [Lumi-supercomputer/LUMI-AI-Guide (Section 03)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/03-file-formats) | Guide for LUMI (hosted by CSC in Finland) |
| Data Storage | [Lumi-supercomputer/LUMI-AI-Guide (Section 04)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/04-data-storage) | Guide for LUMI (hosted by CSC in Finland) |
| Storage and Data Pipelines | [Minerva-guidebook/1 Infrastructure Foundations for Scalable LLM Training (1.3)](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide1_Infrastructure_Foundations/Guide1_Infrastructure_Foundations.html#storage-and-data-pipelines) | A section on working on distributed filesystems from the best practises guidebook by Minerva 4 AI. |

## Evaluation frameworks

Benchmarking and evaluating trained models.

| Topic | Guide | Notes |
| --- | --- | --- |
| LM Eval Harness on LUMI | [LumiOpen/lm-evaluation-harness](https://github.com/LumiOpen/lm-evaluation-harness) | Fork by LumiOpen for LUMI (hosted by CSC in Finland) |
| Evaluation and Model Monitoring | [Minerva-guidebook/ 2 Efficient and Reliable LLM Pretraining (2.11)](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide2_Efficient_Reliable_Pretraining/Guide2_Efficient_Reliable_Pretraining.html#evaluation-and-model-monitoring) | A section on LLM evaluation from the best practises guidebook by Minerva 4 AI. |

## Hyperparameter optimization

Searching hyperparameters at scale on HPC.

| Topic | Guide | Notes |
| --- | --- | --- |
| HPO on HPC | [AaltoRSE/hpo-on-hpc](https://github.com/AaltoRSE/hpo-on-hpc) | |

## Inference

Serving and running inference with trained models.

| Topic | Guide | Notes |
| --- | --- | --- |
| vLLM | [Lumi-supercomputer/LUMI-AI-Guide (Section 10)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/10-LLM-inference) | Guide for LUMI (hosted by CSC in Finland) |
| vLLM | [CSCfi/ai-inference-examples](https://github.com/CSCfi/ai-inference-examples) | Code snippets for Roihu (CSC, Finland) and LUMI (hosted by CSC in Finland); not a full guide |
| Ollama | [CSCfi/ai-inference-examples](https://github.com/CSCfi/ai-inference-examples) | Code snippets for Roihu (CSC, Finland) and LUMI (hosted by CSC in Finland); not a full guide |
| vLLM (multi-node / multi-GPU) | [EPICURE How-To: Multi-Node & Multi-GPU Inference with vLLM](https://eurohpcsupport.eu/how-to-guide/multi-node-multi-gpu-inference-with-vllm/) | Serving a large LLM (Qwen) across nodes on MeluXina (A100) with tensor + pipeline parallelism. |
| llama.cpp (LLM inference on Arm) | [EPICURE: LLM with llama.cpp on Deucalion](https://eurohpcsupport.eu/code-snippet/llm-using-llama/) | Running Llama 3.1 8B with llama.cpp on Deucalion's Arm partition. |
| vLLM | [SURF-ML/vllm-inference-slurm](https://github.com/SURF-ML/vllm-inference-slurm) | For Snellius (SURF, Netherlands). |
| vLLM vs Triton (benchmark) | [cyfronet/Benchmark-Triton-vLLM](https://github.com/cyfronet/Benchmark-Triton-vLLM) | For PLGrid Helios (GH200, Poland). |
| Efficient Inference and Test-Time Compute | [Minerva-guidebook/3 Post-Training — Alignment and User-Centered Objectives (3.3)](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide3_PostTraining_Alignment/Guide3_PostTraining_Alignment.html#efficient-inference-and-test-time-compute) | A section on efficient inference, including reasoning, latency, memory, prompt templating, quantization and pruning, from the the best practises guidebook by Minerva 4 AI. |

## LLM fine-tuning

Fine-tuning large language models, from single-GPU examples to very large training runs.

| Topic | Guide | Notes |
| --- | --- | --- |
| Hugging Face Accelerate | [sweden-ai-factory/llm_finetuning_example](https://github.com/sweden-ai-factory/llm_finetuning_example) | Code snippets for Leonardo, LUMI (hosted by CSC in Finland), and Meluxina |
| Hugging Face Accelerate | [CSCfi/llm-fine-tuning-examples](https://github.com/CSCfi/llm-fine-tuning-examples) | Code snippets for LUMI (hosted by CSC in Finland) |
| DeepSpeed | [AaltoRSE/llm-on-lumi](https://github.com/AaltoRSE/llm-on-lumi/tree/main) | Code snippets for LUMI (hosted by CSC in Finland) |
| Nanotron | [AaltoRSE/llm-on-lumi](https://github.com/AaltoRSE/llm-on-lumi/tree/main) | Code snippets for LUMI (hosted by CSC in Finland) |
| Megatron-Bridge (very large training runs) | [OpenEuroLLM/Megatron-Bridge-LUMI](https://github.com/OpenEuroLLM/Megatron-Bridge-LUMI/tree/main) | The code in this repo has been modified to work on AMD GPUs. See [quickstart](https://github.com/OpenEuroLLM/Megatron-Bridge-LUMI/blob/main/quickstart.md) for instructions on how to run this on LUMI (hosted by CSC in Finland). See also [OpenEuroLLM/Megatron-Bridge-utils](https://github.com/OpenEuroLLM/Megatron-Bridge-utils). Note that this probably requires some work to get it to run and thus probably only relevant for advanced users. |
| Reinforcement learning fine-tuning (GRPO / RLVR) | [CSCfi/llm-rl-fine-tuning-examples](https://github.com/CSCfi/llm-rl-fine-tuning-examples) | Code snippets for LUMI (hosted by CSC in Finland); uses [verl](https://github.com/verl-project/verl) |
| End-to-end LLM finetuning pipeline (LUMI) | [CSCfi/climate-llm-finetuning](https://github.com/CSCfi/climate-llm-finetuning) | On LUMI (hosted by CSC in Finland): data scraping/preprocessing → FAISS/RAG QA-dataset generation → fine-tuning → evaluation |
| Large-scale LLM fine-tuning (FSDP2) | [idriscnrs/Democratizing-LLM-FT](https://github.com/idriscnrs/Democratizing-LLM-FT) | For Jean Zay (IDRIS, France). |
| Megatron-LM pretraining setup | [SURF-ML/Megatron-LM-Snellius](https://github.com/SURF-ML/Megatron-LM-Snellius) | For Snellius (SURF, Netherlands). |
| Instruction tuning & reinforcement learning | [Minerva-guidebook/3 Post-Training — Alignment and User-Centered Objectives (3.1 & 3.2)](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide3_PostTraining_Alignment/Guide3_PostTraining_Alignment.html) | Sections on instruction tuning and reinforcement learning from the best practises guidebook by Minerva 4 AI. |

## MLOps

Experiment tracking and visualization.

| Topic | Guide | Notes |
| --- | --- | --- |
| TensorBoard | [Lumi-supercomputer/LUMI-AI-Guide (Section 07)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/07-TensorBoard-visualization) | |
| MLflow | [docs.csc.fi/support/tutorials/ml-workflows/](https://docs.csc.fi/support/tutorials/ml-workflows/#mlflow); [Lumi-supercomputer/LUMI-AI-Guide (Section 08)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/08-MLflowlization) | Guides for LUMI (hosted by CSC in Finland) |

## Multi GPU and node training

Scaling training across multiple GPUs and nodes.

| Topic | Guide | Notes |
| --- | --- | --- |
| PyTorch DDP | [Lumi-supercomputer/LUMI-AI-Guide (Section 05)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/05-multi-gpu-and-node) | Guide for LUMI (hosted by CSC in Finland) |
| PyTorch DeepSpeed | [Lumi-supercomputer/LUMI-AI-Guide (Section 05)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/05-multi-gpu-and-node) | Guide for LUMI (hosted by CSC in Finland) |
| Hugging Face Accelerate | [CSCfi/llm-fine-tuning-examples](https://github.com/CSCfi/llm-fine-tuning-examples) | Code snippets for LUMI (hosted by CSC in Finland) |
| torchrun single-node multi-GCD | [Getting_Started_with_AI_workshop (Ch. 08)](https://github.com/Lumi-supercomputer/Getting_Started_with_AI_workshop/tree/main/08_Scaling_to_multiple_GPUs) | Workshop material. Adapting a Hugging Face/PyTorch training script for data-parallel training across all 8 GCDs on one node via torchrun. |
| Multi-node scaling (RCCL/interconnect) | [Getting_Started_with_AI_workshop (Ch. 09)](https://github.com/Lumi-supercomputer/Getting_Started_with_AI_workshop/tree/main/09_Extreme_scale_AI) | Workshop material. Multi-node scaling: CPU–GPU binding masks, `NCCL_SOCKET_IFNAME`/`NCCL_NET_GDR_LEVEL`, aws-ofi-nccl CXI plugin for RCCL. |
| PyTorch DDP multi-node scaling | [EPICURE: Scaling PyTorch DDP on Vega](https://eurohpcsupport.eu/best-practice/best-practice-guide-to-scaling-pytorch-distributeddataparallel/) | For Vega (A100). |
| Scaling AI workloads (multiple EuroHPC systems) | [EPICURE: Best Practice Guide on AI on EuroHPC Systems](https://eurohpcsupport.eu/best-practice/best-practice-guide-on-artificial-intelligence-on-eurohpc-systems/); code: [opencode.it4i.eu/epicure/bpg-ai-workflows](https://opencode.it4i.eu/epicure/bpg-ai-workflows) | Vision and language benchmarks across 8 EuroHPC systems: Deucalion, Jupiter, Karolina, Leonardo, LUMI, MeluXina, MN5, Vega. |
| PyTorch DDP / Lightning / DeepSpeed examples | [CSCfi/pytorch-ddp-examples](https://github.com/CSCfi/pytorch-ddp-examples) | For Roihu (CSC, Finland). |
| LLM pretraining at scale | [Minerva-guidebook/2  Efficient and Reliable LLM Pretraining](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide2_Efficient_Reliable_Pretraining/Guide2_Efficient_Reliable_Pretraining.html) | A section on pretraining, including parallelism techniques and training efficiency, from best practises guidebook by Minerva 4 AI. |

## Profiling

Monitoring and profiling GPU utilization and performance.

| Topic | Guide | Notes |
| --- | --- | --- |
| ROCm-SMI on LUMI | [Lumi-supercomputer/LUMI-AI-Guide (Section 06)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/06-monitoring-and-profiling) | Guide for LUMI (hosted by CSC in Finland) |
| PyTorch Profiler | [Lumi-supercomputer/LUMI-AI-Guide (Section 06)](https://github.com/Lumi-supercomputer/LUMI-AI-Guide/tree/main/06-monitoring-and-profiling) | |
| Python & GPU profiling | [EPICURE How-To: Profile your Python Code (cProfile to GPU timelines)](https://eurohpcsupport.eu/how-to-guide/how-to-profile-your-python-code-from-cprofile-to-gpu-timelines/) | Profiling Python from cProfile through to GPU timelines. |

## Quantization

Reducing model size and memory footprint via quantization.

| Topic | Guide | Notes |
| --- | --- | --- |
| AWQ (Activation-aware Weight Quantization) | [docs.csc.fi/support/tutorials/ml-llm/](https://docs.csc.fi/support/tutorials/ml-llm/#using-awq-quantization-via-llm-compressor); [CSCfi/llm-quantization-scripts](https://github.com/CSCfi/llm-quantization-scripts) | Examples for LUMI (hosted by CSC in Finland) and Roihu (CSC, Finland) |
| bitsandbytes | [docs.csc.fi/support/tutorials/ml-llm/](https://docs.csc.fi/support/tutorials/ml-llm/#using-bitsandbytes-quantization); [CSCfi/llm-quantization-scripts](https://github.com/CSCfi/llm-quantization-scripts) | Examples for LUMI (hosted by CSC in Finland) and Roihu (CSC, Finland) |
| GPTQ (Gradient Post-training Quantization) | [docs.csc.fi/support/tutorials/ml-llm/](https://docs.csc.fi/support/tutorials/ml-llm/#using-gptq-quantization); [CSCfi/llm-quantization-scripts](https://github.com/CSCfi/llm-quantization-scripts) | Examples for LUMI (hosted by CSC in Finland) and Roihu (CSC, Finland) |

## Relevant topics where no material has been found

Topics we would like to cover but have not yet found good material for:

- Data Preprocessing on HPC
- Moving from HPC to production environments

## Relevant resources that need to be mapped

Promising resources we have found but not yet sorted into the sections above.

- [gitlab.tuwien.ac.at/vsc-public/training/LLMs-on-supercomputers](https://gitlab.tuwien.ac.at/vsc-public/training/LLMs-on-supercomputers)
- [amd/HPCTrainingExamples/tree/main/MLExamples](https://github.com/amd/HPCTrainingExamples/tree/main/MLExamples)
- [ENCCS/castiel-multi-gpu-ai](https://github.com/ENCCS/castiel-multi-gpu-ai)
- [openhackathons-org/End-to-End-AI-for-Science/tree/main/workspace/python](https://github.com/openhackathons-org/End-to-End-AI-for-Science/tree/main/workspace/python)
- [olcf/ai-training-series](https://github.com/olcf/ai-training-series)
- [Minerva-guidebook/4 Explainable AI](https://best-practice-guides.minerva4ai.eu/optimizing-ai-models-on-european-infrastructure/Guide4_Explainable_AI/Guide4_Explainable_AI.html)

## HPC centre sources

A country-by-country list of European HPC centre, EuroHPC hosting site, and AI Factory GitHub/GitLab organizations whose training material and examples we still want to review and map into the sections above. Contributions and additions are welcome.

See [hpc-centre-sources.md](hpc-centre-sources.md).

## License

This collection is licensed under the [MIT License](LICENSE).

## Acknowledgements

This collection is maintained by the [LUMI AI Factory](https://lumi-ai-factory.eu).

[![LUMI AI Factory](assets/images/LUMI_AIF_logo.png)](https://lumi-ai-factory.eu)

[![Funded by the EuroHPC Joint Undertaking and Participating States](assets/images/LUMI_AIF_funding.png)](https://lumi-ai-factory.eu)
