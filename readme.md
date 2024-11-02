# APrompt 🤖

![Project Banner](readme_files/banner.png)

An automated prompt engineering tool for Large Language Models (LLMs), designed for universal domain adaptation.

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## ✨ Features

- 🚀 Simple and intuitive prompt creation
- 🔄 Reusable prompt templates
- 🌐 Multi-language support

## 🚀 Quick Start

### 1. Configure Your Environment ⚙️

Create a configuration file `config.yaml`:

```yaml
openai:
  api_key: " "
  base_url: ' '
```

### 2. Define Your Prompt Template 📝

Create a prompt template file `meta.yaml`:
```yaml
prompt: |
  User problem：{question}

requirements: |
  ...

faq:
  - question: "..."
    answer: |
      ...

  - question: "..."
    answer: |
      ...
```

### 3. Implement the Optimizer 🔧

Use `main.py` to execute:
```python
optimizer = Optimizer(
    optimized_path="workspace",
    initial_round=1,
    max_rounds=30,
    name="your_prompt_name",
)
# Optimize workflow via setting the optimizer's mode to 'Graph'
optimizer.optimize()
```

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

---

<p align="center">Made with ❤️ by the APrompt and AFlow Team</p>