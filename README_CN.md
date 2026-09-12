<p align="left">
   <a href="README.md">English</a>&nbsp;｜&nbsp;中文
</p>
<br>

# Atria Dawn Preview: 从研究问题到可验证的结果

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
    <img alt="Twitter Follow" src="https://img.shields.io/badge/Twitter-Atria Dawn Preview-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<div align="center" style="line-height: 1;">
  <a href="LICENSE" style="margin: 2px;">
    <img alt="License" src="https://img.shields.io/badge/License-MIT-blue" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<p align="center">
  <a href="https://atria-asi.com/">🖥️<b>官方网站</b></a>
  <a href="https://github.com/atria-asi/Atria-Dawn-Preview">💬<b>GitHub</b></a>
</p>

## 介绍

Atria Dawn Preview 是由上海人工智能实验室研发的新一代智能体大模型预览版，模型基于744B MoE基座进行训练，面向需要持续理解环境、调用工具并完成多步任务的研究与工程场景。该模型旨在协助用户将开放性问题推进为可执行、可验证和可复现的结果。模型能够结合任务目标与环境反馈，参与问题分析、方案设计、工具调用、代码实现、实验执行、结果分析以及失败恢复等环节。

Atria Dawn Preview 从以下四个维度赋能智能体任务，重点强化了在科研自动化、办公等真实生产力场景下的端到端交付能力。

- **Discovery：** 检索和组织证据，开展深度研究，并将研究问题转化为可执行的实验方案。
- **Creation：** 构建软件、交互应用、游戏、数据可视化和机器学习系统。
- **Delivery：** 将文档、数据和设计要求转化为报告、演示文稿及其他结构化成果。
- **Cybersecurity：** 在经过授权的环境中分析安全问题、验证漏洞、实施修复并完成复验。



## 模型下载

<div align="center">

| **模型名** | **简介** | **Hugging Face** | **ModelScope** |
| :---: | :---: | :---: | :---: |
| Atria-Dawn-Preview | Instruct 模型 | [Model](https://huggingface.co/internlm/Atria-Dawn-Preview) | [Model](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/Atria-Dawn-Preview) |
| Atria-Dawn-Preview-FP8 | FP8量化Instruct模型 | [Model](https://huggingface.co/internlm/Atria-Dawn-Preview-FP8) | [Model](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/Atria-Dawn-Preview-FP8) |

</div>


## 性能评估
我们对Atria Dawn Preview进行了全面评估。以下是部分评测结果。


<div align="center">
  <img src="assets/evaluation.png" width="100%" alt="Atria Dawn Preview Evaluation Results" />
</div>
<!-- todo: 柱状图注释 -->

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

在此补充本地运行、推理服务和环境配置说明。

```bash
# 在此添加安装和运行命令。
``` -->

## 许可证

本仓库的代码和权重依照MIT协议开源。

<!-- ## Citation

```text
在此添加正式引用信息。
``` -->

## 联系我们
如有问题或建议，欢迎通过邮件或github等平台联系我们。