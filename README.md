<p align="left">
    <a href="README_CN.md">中文</a>&nbsp;｜&nbsp;English
</p>
<br>

# Atria Dawn Preview: From Research Questions To Verifiable Results

<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->
<!-- markdownlint-disable no-duplicate-header -->

<div align="center">
  <img src="assets/atria.png" width="60%" alt="Atria Dawn Preview" />
</div>
<hr>

<div align="center" style="line-height: 1;">
  <a href="https://huggingface.co/internlm/Atria-Dawn-Preview" target="_blank" style="margin: 2px;">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Atria Dawn Preview-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://www.modelscope.cn/models/Shanghai_AI_Laboratory/Atria-Dawn-Preview" target="_blank" style="margin: 2px;">
    <img alt="ModelScope" src="https://img.shields.io/badge/ModelScope-Atria Dawn Preview-blue?logo=ModelScope" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>

<div align="center" style="line-height: 1;">
  <a href="https://x.com/AtriaASI" target="_blank" style="margin: 2px;">
    <img alt="Twitter Follow" src="https://img.shields.io/badge/Twitter-Atria Dawn Preview-blue?logo=x" style="display: inline-block; vertical-align: middle;"/>
  </a>
<a href="https://discord.gg/jT8SDt8up" target="_blank" style="margin: 2px;">
    <img alt="Discord" src="https://img.shields.io/badge/Discord-Atria Dawn Preview-blue?logo=discord" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>

<div align="center" style="line-height: 1;">
  <a href="LICENSE" style="margin: 2px;">
    <img alt="License" src="https://img.shields.io/badge/License-MIT-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<p align="center">
  <a href="https://atria-asi.ai/">🖥️<b>Website</b></a>
  <a href="https://github.com/atria-asi/Atria-Dawn-Preview">💬<b>GitHub</b></a>
</p>

## Introduction

Atria Dawn Preview is a preview version of a new-generation agentic model developed by the Shanghai Artificial Intelligence Laboratory. Built on the 744B-parameter MoE GLM-5.2 foundation model, it is designed for research and engineering scenarios that require continuous environmental understanding, tool use, and multi-step task completion. The model helps users drive open-ended problems toward executable, verifiable, and reproducible results. It can support problem analysis, solution design, tool use, code implementation, experiment execution, result analysis, and failure recovery by combining task objectives with environmental feedback.

Atria Dawn Preview empowers agentic tasks across four dimensions, with a particular focus on end-to-end delivery in real-world productivity scenarios such as scientific automation and office work:

- **Discovery:** Retrieving and organizing evidence, conducting deep research, and turning research questions into executable experimental plans.
- **Creation:** Building software, interactive applications, games, data visualizations, and machine learning systems.
- **Delivery:** Transforming documents, data, and design requirements into reports, presentations, and other structured deliverables.
- **Cybersecurity:** Analyzing security issues, validating vulnerabilities, applying fixes, and performing re-validation in authorized environments.

## Model Downloads

<div align="center">

| **Model** | **Description** | **Context** | **Hugging Face** | **ModelScope** |
| :---: | :---: | :---: | :---: |
| Atria-Dawn-Preview | Instruct model | [Model](https://huggingface.co/internlm/Atria-Dawn-Preview) | [Model](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/Atria-Dawn-Preview) |
| Atria-Dawn-Preview-FP8 | FP8-quantized Instruct model | [Model](https://huggingface.co/internlm/Atria-Dawn-Preview-FP8) | [Model](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/Atria-Dawn-Preview-FP8) |

</div>

## Evaluation Results

We conducted a comprehensive evaluation of Atria Dawn Preview. The table below presents benchmark results.

<div align="center">
  <img src="assets/evaluation.png" width="100%" alt="Atria Dawn Preview Evaluation Results" />
</div>
<!-- TODO: Add chart annotations. -->

<div align="center">

| Benchmark | Atria Dawn Preview | DeepSeek V4 Pro 0813 | KIMI K3 | Qwen 3.8 Max | GLM 5.3 | GPT 5.6 sol | Claude Opus 5 |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| AutomationBench | 53.8 | 41.7 | 45.9 | 49.7 | 49.2 | 45.7 | 49.4 |
| BFCL v4 | 77.0 | 71.4 | 69.1 | - | 74.1 | - | - |
| CyberGym | 86.5 | 83.3 | 78.7 | 73.8 | 84.5 | 83.6 | - |
| DeepSearchQA | 96.0 | - | 95.9 | - | 94.7 | 93.2 | - |
| Workspace-Bench-Lite | 68.2 | 58.1 | 65.8 | 67.4 | 67.7 | 60.5 | 70.1 |
| BrowseComp | 92.5 | 83.4 | 91.2 | - | - | 92.2 | 90.8 |
| SkillsBench | 66.4 | 65.0 | 51.9 | 66.7 | 63.3 | 62.5 | 63.7 |
| Workspace-Bench | 65.0 | 55.7 | 60.6 | 63.9 | 63.9 | 56.0 | 65.8 |
| MLE-bench Lite | 86.2 | 86.8 | 85.8 | 81.3 | 80.8 | 88.9 | 88.0 |
| WideSearch | 81.9 | - | 79.6 | 81.9 | 82.7 | 83.3 | - |
| DeepResearch Bench II | 51.1 | 46.6 | 51.3 | 49.2 | 52.7 | 50.7 | 54.1 |
| τ³-Bench Banking | 41.2 | 44.3 | 37.1 | 55.2 | 40.2 | 46.9 | 48.7 |
| Terminal-Bench 2.1 | 78.3 | 78.7 | - | 89.3 | 85.4 | 85.1 | 90.2 |
| GDPval | 1583 | 1517 | 1611 | 1722 | 1667 | 1682 | 1768 |
| SWE-bench Pro | 59.6 | 58.3 | 61.6 | 65.1 | 60.3 | 61.4 | 74.7 |
| JobBench | 50.3 | 54.1 | 54.3 | 52.7 | 58.2 | 45.4 | 68.0 |

</div>

<!-- ## How to Run Locally

Add instructions for local inference, deployment, and environment setup here.

```bash
# Add installation and launch commands here.
``` -->

## Deployment & Online Access

Atria Dawn Preview supports both local deployment and hosted access. For online access, use the service corresponding to your region.

| Region            | Access                                                                | Tutorial                                                                  |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| **International** | [Link](https://api.atria-asi.ai/)                                     | [Tutorial](https://api.atria-asi.ai/docs)                                 |
| **China**         | [Link](https://discovery.intern-ai.org.cn/token-plan/home?tabIndex=0) | [Tutorial](https://discovery.intern-ai.org.cn/token-plan/home?tabIndex=3) |

For local deployment, please refer to the following deployment guides.

- [SGLang](https://github.com/sgl-project/sglang) (v0.5.13.post1+) — see [cookbook](https://cookbook.sglang.io/autoregressive/GLM/GLM-5.2)
- [vLLM](https://github.com/vllm-project/vllm) (v0.23.0+) — see [recipes](https://recipes.vllm.ai/zai-org/GLM-5.2)

## License

The code and model weights in this repository are released under the MIT License.

<!-- ## Citation

```text
Add the official citation here.
``` -->

## Contact

For questions or suggestions, please contact us by email or through GitHub and other project platforms.
