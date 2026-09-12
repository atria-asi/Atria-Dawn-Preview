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
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Atria%20Dawn%20Preview-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://www.modelscope.cn/models/Shanghai_AI_Laboratory/Atria-Dawn-Preview" target="_blank" style="margin: 2px;">
    <img alt="ModelScope" src="https://img.shields.io/badge/ModelScope-Atria%20Dawn%20Preview-blue?logo=ModelScope" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<div align="center" style="line-height: 1;">
  <a href="https://x.com/AtriaASI" target="_blank" style="margin: 2px;">
    <img alt="Twitter Follow" src="https://img.shields.io/badge/Twitter-Atria%20Dawn%20Preview-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<div align="center" style="line-height: 1;">
  <a href="LICENSE" style="margin: 2px;">
    <img alt="License" src="https://img.shields.io/badge/License-MIT-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<p align="center">
  <a href="https://atria-asi.com/">🖥️<b>Website</b></a>
  <a href="https://github.com/atria-asi/Atria-Dawn-Preview"> 💬<b>GitHub</b></a>
</p>

## Introduction

Atria Dawn Preview is a preview version of a new-generation agentic model developed by the Shanghai Artificial Intelligence Laboratory. Trained on a 744B-parameter MoE foundation model, it is designed for research and engineering scenarios that require continuous environmental understanding, tool use, and multi-step task completion. The model helps users drive open-ended problems toward executable, verifiable, and reproducible results. It can support problem analysis, solution design, tool use, code implementation, experiment execution, result analysis, and failure recovery by combining task objectives with environmental feedback.

Atria Dawn Preview empowers agentic tasks across four dimensions, with a particular focus on end-to-end delivery in real-world productivity scenarios such as scientific automation and office work:

- **Discovery:** Retrieving and organizing evidence, conducting deep research, and turning research questions into executable experimental plans.
- **Creation:** Building software, interactive applications, games, data visualizations, and machine learning systems.
- **Delivery:** Transforming documents, data, and design requirements into reports, presentations, and other structured deliverables.
- **Cybersecurity:** Analyzing security issues, validating vulnerabilities, applying fixes, and performing re-validation in authorized environments.

## Model Downloads

<div align="center">

| **Model** | **Description** | **Hugging Face** | **ModelScope** |
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
| AutomationBench | 54.5 | 27.3 | 45.9 | 49.7 | 49.2 | 45.7 | 49.4 |
| BFCL v4 | 77.0 | 71.4 | 69.1 | - | 74.1 | - | - |
| CyberGym | 86.5 | 73.8 | 78.7 | 73.8 | 84.5 | 83.6 | - |
| DeepSearchQA | 96.0 | - | 95.9 | - | 94.7 | 93.2 | - |
| Workspace-Bench-Lite | 68.2 | 58.1 | 65.8 | 67.4 | 67.7 | 60.5 | 70.1 |
| BrowseComp | 92.5 | 83.4 | 91.2 | - | - | 92.2 | 90.8 |
| SkillsBench | 66.4 | 65.0 | 51.9 | 66.7 | 63.3 | 62.5 | 63.7 |
| WorkspaceBench | 65.0 | 55.7 | 60.6 | 63.9 | 63.9 | 56.0 | 65.8 |
| MLE-bench Lite | 86.2 | 86.8 | 85.8 | 81.3 | 80.8 | 88.9 | 88.0 |
| WideSearch | 81.9 | - | 79.6 | 81.9 | 82.7 | 83.3 | - |
| DeepResearch Bench II | 51.1 | 46.6 | 51.3 | 49.2 | 52.7 | 50.7 | 54.1 |
| τ³-Bench Banking | 40.5 | 49.2 | 39.9 | 50.8 | 42.8 | 42.0 | 47.9 |
| Terminal-Bench 2.1 | 78.3 | 78.7 | - | 89.3 | 85.4 | 85.1 | 90.2 |
| GDPval | 66.4 | 52.7 | 65.5 | 75.9 | 68.2 | 69.6 | 80.0 |
| SWE-bench Pro | 59.6 | 58.3 | 61.6 | 65.1 | 60.3 | 61.4 | 74.7 |
| JobBench | 50.3 | 54.1 | 54.3 | 52.7 | 58.2 | 45.4 | 68.0 |

</div>

<!-- ## How to Run Locally

Add instructions for local inference, deployment, and environment setup here.

```bash
# Add installation and launch commands here.
``` -->

## License

The code and model weights in this repository are released under the MIT License.

<!-- ## Citation

```text
Add the official citation here.
``` -->

## Contact

For questions or suggestions, please contact us by email or through GitHub and other project platforms.
