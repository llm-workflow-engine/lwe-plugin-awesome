# LLM Workflow Engine (LWE) Awesome plugin

Awesome plugin for [LLM Workflow Engine](https://github.com/llm-workflow-engine/llm-workflow-engine)

Use prompts from [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts)

## Installation

### From packages

Install the latest version of this software directly from github with pip:

```bash
pip install git+https://github.com/llm-workflow-engine/lwe-plugin-awesome
```

### From source (recommended for development)

Install the latest version of this software directly from git:

```bash
git clone https://github.com/llm-workflow-engine/lwe-plugin-awesome.git
```

Install the development package:

```bash
cd lwe-plugin-awesome
pip install -e .
```

## Configuration

Add the following to `config.yaml` in your profile:

```yaml
plugins:
  enabled:
    - awesome
    # Any other plugins you want enabled...
  # These are the default values.
  awesome:
    prompts:
      uri: 'https://github.com/f/awesome-chatgpt-prompts/raw/main/prompts.csv'
      temp_filename: 'awesome-prompts.csv'
```

## Usage

From a running LWE shell...

To reload the prompts:

```
/awesome reload
```

To use a prompt (this will open the prompt in an editor for further adjustment before submission to the LLM):

```
/awesome Linux Terminal
```
