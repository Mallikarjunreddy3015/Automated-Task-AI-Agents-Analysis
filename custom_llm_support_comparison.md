# AI Agent Frameworks Comparison: Custom LLM API Support

## Overview
This document analyzes the custom LLM API support capabilities of various AI agent frameworks, focusing on their flexibility in integrating with different language models beyond their default options.

## Open-Source Frameworks

### LangGraph
- **Custom LLM Support**: Excellent
- **Compatible Models**: OpenAI, Anthropic, Mistral, Llama, local models via Ollama
- **Integration Method**: Modular design allows swapping LLM providers through configuration
- **API Requirements**: Requires API keys for commercial models, supports local deployment
- **Limitations**: Some advanced features may work best with specific models

### OpenAI Agents SDK
- **Custom LLM Support**: Limited
- **Compatible Models**: Primarily OpenAI models (GPT-4o, GPT-o3)
- **Integration Method**: Tightly coupled with OpenAI's ecosystem
- **API Requirements**: Requires OpenAI API key
- **Limitations**: Not designed for non-OpenAI models

### Smolagents
- **Custom LLM Support**: Good
- **Compatible Models**: Hugging Face models, OpenAI, Anthropic, compatible with most API-based LLMs
- **Integration Method**: Simple configuration for model switching
- **API Requirements**: Requires appropriate API keys
- **Limitations**: Performance may vary with different models

### CrewAI
- **Custom LLM Support**: Very Good
- **Compatible Models**: OpenAI, Anthropic, Mistral, Llama, and others
- **Integration Method**: Flexible model configuration per agent
- **API Requirements**: Requires API keys for commercial models
- **Limitations**: Some advanced features may require specific model capabilities

### AutoGen
- **Custom LLM Support**: Excellent
- **Compatible Models**: Wide range including OpenAI, Azure OpenAI, Anthropic, Hugging Face models
- **Integration Method**: Modular design with pluggable LLM interfaces
- **API Requirements**: Requires appropriate API keys
- **Limitations**: Complex setups may require additional configuration

### Semantic Kernel
- **Custom LLM Support**: Very Good
- **Compatible Models**: OpenAI, Azure OpenAI, Hugging Face models, custom endpoints
- **Integration Method**: Abstracted connectors for different providers
- **API Requirements**: Requires appropriate API keys, optimized for Azure
- **Limitations**: Some features work best within Microsoft ecosystem

### LlamaIndex Agents
- **Custom LLM Support**: Good
- **Compatible Models**: OpenAI, Anthropic, local models, custom endpoints
- **Integration Method**: Configurable LLM settings
- **API Requirements**: Requires appropriate API keys
- **Limitations**: Retrieval performance may vary with different models

## Commercial Platforms

### Claude AI Agents (Anthropic)
- **Custom LLM Support**: None
- **Compatible Models**: Claude models only
- **Integration Method**: N/A
- **API Requirements**: Anthropic API access
- **Limitations**: Locked to Anthropic's ecosystem

### GenSpark Super Agent
- **Custom LLM Support**: Limited
- **Compatible Models**: Primarily uses proprietary mixture of models
- **Integration Method**: Limited configuration options
- **API Requirements**: Subscription includes API access
- **Limitations**: Cannot fully customize model selection

### Manus AI
- **Custom LLM Support**: None
- **Compatible Models**: Proprietary models only
- **Integration Method**: N/A
- **API Requirements**: Included in subscription
- **Limitations**: Closed ecosystem

### Orby
- **Custom LLM Support**: Limited
- **Compatible Models**: Primarily uses proprietary models
- **Integration Method**: Some configuration options
- **API Requirements**: Included in platform
- **Limitations**: Limited customization

### Zapier AI
- **Custom LLM Support**: None
- **Compatible Models**: Proprietary implementation
- **Integration Method**: N/A
- **API Requirements**: Included in subscription
- **Limitations**: Cannot change underlying models

## Open-Source Alternatives to Manus AI

### OpenManus
- **Custom LLM Support**: Excellent
- **Compatible Models**: OpenAI, Anthropic, potentially others through configuration
- **Integration Method**: Configuration file customization
- **API Requirements**: Requires API keys for chosen providers
- **Limitations**: May require code modifications for some models

### Suna
- **Custom LLM Support**: Excellent
- **Compatible Models**: Anthropic, Daytona, Firecrawl, Tavli, and others
- **Integration Method**: Flexible configuration
- **API Requirements**: Requires API keys for chosen providers
- **Limitations**: Performance depends on model quality
