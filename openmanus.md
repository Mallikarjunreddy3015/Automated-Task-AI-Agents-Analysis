# OpenManus: Open Source Alternative to Manus AI

## Overview
OpenManus is a fully open-source alternative to Manus AI, designed to democratize access to autonomous AI agents. While Manus AI requires an invitation code, OpenManus breaks down barriers by providing a powerful framework that's freely available to everyone. Developed by the MetaGPT research team, it allows users to create AI agents capable of executing complex tasks with minimal human input.

## Key Features

### Modular and Extensible Architecture
- Customizable and extensible functionality based on specific needs
- Flexible framework adaptable for various use cases
- Not constrained by rigid structures

### No Invite Code Required
- Freely available to everyone
- No waitlist or invitation process
- No enterprise-only features
- Democratized access for individual developers, researchers, and organizations of all sizes

### Advanced Autonomous Capabilities
- Makes informed decisions based on available data
- Interacts meaningfully with users through natural language
- Executes complex tasks independently
- Learns from past interactions to improve performance

### Open-Source Community
- Benefits from community contributions
- Continuous improvement and adaptation to emerging needs and technologies

## Installation Methods

### Method 1: Using Conda
```bash
conda create -n open_manus python=3.12
conda activate open_manus
git clone https://github.com/mannaandpoem/OpenManus.git
cd OpenManus
pip install -r requirements.txt
```

### Method 2: Using UV (Recommended)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
git clone https://github.com/mannaandpoem/OpenManus.git
cd OpenManus
uv venv --python 3.12
source .venv/bin/activate
uv pip install -r requirements.txt
```

## Configuration
OpenManus requires configuration for the LLM APIs it uses:
```toml
[Global]
# llm model
llm = "gpt-4o"
base_url = "https://api.openai.com/v1"
api_key = "sk-..." # Replace with your actual API key
# max_tokens = 4096
temperature = 0.0

[Global.vision]
# llm vision model
llm = "gpt-4o"
base_url = "https://api.openai.com/v1"
api_key = "sk-..." # Replace with your actual API key
```

## Custom LLM Support
- Supports OpenAI models by default
- Can be configured to use custom LLM APIs by modifying the configuration file
- Requires API keys for the chosen LLM provider

## OpenManus-RL: Reinforcement Learning Extension
- Enhances AI agents using reinforcement learning techniques
- Developed collaboratively by researchers from UIUC and the OpenManus team
- Implements methods like GRPO (Generalized Reinforcement Policy Optimization)
- Improves agent performance through enhanced decision making
- Supports training agents across various environments to improve adaptability
- Allows fine-tuning LLM-based agents for specific tasks through systematic reinforcement

## Real-World Applications
- Web development and maintenance
- Research and data analysis
- Content creation and management
- Business intelligence and market analysis
- Workflow automation

## Cost
- Free and open-source
- Users only pay for the LLM API usage (e.g., OpenAI API costs)
- No subscription fees or usage limits imposed by OpenManus itself
