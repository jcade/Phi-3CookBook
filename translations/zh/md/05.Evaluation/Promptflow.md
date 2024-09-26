# **介绍 Promptflow**

[Microsoft Prompt Flow](https://microsoft.github.io/promptflow/index.html?WT.mc_id=aiml-138114-kinfeylo) 是一个可视化的工作流自动化工具，允许用户使用预构建模板和自定义连接器创建自动化工作流。它旨在帮助开发人员和业务分析师快速构建数据管理、协作和流程优化等任务的自动化流程。通过 Prompt Flow，用户可以轻松连接不同的服务、应用程序和系统，并自动化复杂的业务流程。

Microsoft Prompt Flow 旨在简化由大型语言模型（LLM）驱动的 AI 应用程序的端到端开发周期。无论你是在构思、原型设计、测试、评估还是部署基于 LLM 的应用程序，Prompt Flow 都能简化这一过程，使你能够构建具有生产质量的 LLM 应用程序。

## 使用 Microsoft Prompt Flow 的主要特点和优势：

**交互式创作体验**

Prompt Flow 提供了流程结构的可视化表示，使你能够轻松理解和导航项目。
它提供了一种类似笔记本的编码体验，以提高流程开发和调试的效率。

**提示变体和调优**

创建和比较多个提示变体，以便进行迭代改进。评估不同提示的性能并选择最有效的提示。

**内置评估流程**

使用内置评估工具评估提示和流程的质量和效果。
了解基于 LLM 的应用程序的表现如何。

**全面的资源**

Prompt Flow 包含内置工具、示例和模板库。这些资源为开发提供了起点，激发了创造力，加速了开发过程。

**协作和企业准备**

支持团队协作，允许多个用户共同处理提示工程项目。
有效维护版本控制和共享知识。简化从开发、评估到部署和监控的整个提示工程过程。

## 在 Prompt Flow 中的评估

在 Microsoft Prompt Flow 中，评估在衡量 AI 模型表现方面起着至关重要的作用。让我们来探讨如何在 Prompt Flow 中自定义评估流程和指标：

![PFVizualise](../../../../translated_images/pfvisualize.e96398930e67b609687d11081caa625eb4313ff62e91998913a9df3cee641688.zh.png)

**理解 Prompt Flow 中的评估**

在 Prompt Flow 中，流程表示处理输入并生成输出的节点序列。评估流程是专门设计用于根据特定标准和目标评估运行性能的特殊类型流程。

**评估流程的关键特点**

它们通常在被测试的流程之后运行，使用其输出。它们计算分数或指标来衡量被测试流程的性能。指标可以包括准确性、相关性分数或任何其他相关度量。

### 自定义评估流程

**定义输入**

评估流程需要接受被测试运行的输出。定义输入与标准流程类似。
例如，如果你在评估一个问答流程，可以将输入命名为“answer”。如果评估一个分类流程，可以将输入命名为“category”。可能还需要实际标签等真实输入。

**输出和指标**

评估流程生成衡量被测试流程性能的结果。可以使用 Python 或 LLM（大型语言模型）计算指标。使用 log_metric() 函数记录相关指标。

**使用自定义评估流程**

开发适合你特定任务和目标的评估流程。根据你的评估目标自定义指标。
将此自定义评估流程应用于批量运行以进行大规模测试。

## 内置评估方法

Prompt Flow 还提供内置评估方法。
你可以提交批量运行，并使用这些方法评估你的流程在大数据集上的表现。
查看评估结果，比较指标，并根据需要进行迭代。
请记住，评估对于确保你的 AI 模型符合预期标准和目标至关重要。查阅官方文档以获取有关在 Microsoft Prompt Flow 中开发和使用评估流程的详细说明。

总之，Microsoft Prompt Flow 通过简化提示工程和提供强大的开发环境，赋能开发人员创建高质量的 LLM 应用程序。如果你正在使用 LLM，Prompt Flow 是一个值得探索的工具。查阅 [Prompt Flow 评估文档](https://learn.microsoft.com/azure/machine-learning/prompt-flow/how-to-develop-an-evaluation-flow?view=azureml-api-2?WT.mc_id=aiml-138114-kinfeylo) 获取有关在 Microsoft Prompt Flow 中开发和使用评估流程的详细说明。

免责声明：本翻译由人工智能模型从原文翻译而来，可能并不完美。
请审阅翻译结果并进行必要的修改。