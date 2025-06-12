# 🤖 ZAI Multi-Provider MCP Server

[![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)](https://github.com/Zrald1/zai-mcp-server)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/node.js-18%2B-brightgreen.svg)](https://nodejs.org/)
[![Free](https://img.shields.io/badge/FREE-No%20License%20Required-brightgreen.svg)](#free)
[![Multi-Provider](https://img.shields.io/badge/Multi--Provider-OpenRouter%20%7C%20Anthropic%20%7C%20DeepSeek-purple.svg)](#providers)

**FREE Multi-Provider AI MCP Server** with support for OpenRouter, Anthropic, and DeepSeek APIs. Features automatic failover, AI-to-AI loops, and smart data collection. **No license validation required** - completely free for all users!

## 💝 **Support Development**

If you find this project helpful, consider supporting development:

### **Crypto Donations**
- **BNB (Binance Smart Chain)**: `0xB8E0b6D4BaaFd1ac4De9245A760cB8F09bB7D084`
- **Bitcoin (BTC)**: `bc1q77k0ju6ta3sp0vm3phm6dek432rzg7cqwf43z6`
- **Ethereum (ETH)**: `0xB8E0b6D4BaaFd1ac4De9245A760cB8F09bB7D084`
- **Polygon (MATIC)**: `0xB8E0b6D4BaaFd1ac4De9245A760cB8F09bB7D084`
- **Dogecoin (DOGE)**: `DGbDQEgJLnNR2yEmWFrusFd7jLya4aoZMA`

Your support helps maintain and improve this open-source project! 🙏

## ✨ **Key Features**

- 🆓 **Completely FREE** - No license validation or restrictions
- 🤖 **Multi-Provider Support** - OpenRouter, Anthropic, DeepSeek APIs
- 🔄 **Automatic Failover** - Smart switching between providers/models
- 🔁 **AI-to-AI Loops** - Infinite improvement cycles
- 📊 **Smart Data Collection** - Contributes to AI model development
- ⚡ **High Availability** - Multiple API keys with rotation
- 🎯 **Quality Filtering** - Only valuable interactions collected
- 🌐 **Global Access** - Works worldwide, no restrictions

## 🚀 **Quick Setup**

### **Option 1: OpenRouter (Recommended - Free Models Available)**
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "OPENROUTER_API_KEY": "sk-or-v1-abc123...,sk-or-v1-def456...,sk-or-v1-ghi789...",
        "MODEL": "deepseek/deepseek-r1-0528:free"
      }
    }
  }
}
```

### **Option 2: Anthropic Claude**
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "ANTHROPIC_API_KEY": "sk-ant-api03-abc123...",
        "MODEL": "claude-3-5-sonnet-20241022"
      }
    }
  }
}
```

### **Option 3: Google Gemini (Advanced Multimodal)**
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "GEMINI_API_KEY": "AIzaSyAbc123...",
        "MODEL": "gemini-2.5-flash-preview-05-20"
      }
    }
  }
}
```

### **Option 4: DeepSeek (Best Value)**
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "DEEPSEEK_API_KEY": "sk-abc123...",
        "MODEL": "deepseek-chat"
      }
    }
  }
}
```

### **Option 5: Multi-Model Voting (AI Consensus)**
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "OPENROUTER_API_KEY": "sk-or-v1-abc123...,sk-or-v1-def456...,sk-or-v1-ghi789...",
        "ANTHROPIC_API_KEY": "sk-ant-api03-abc123...",
        "DEEPSEEK_API_KEY": "sk-abc123...",
        "MODEL": "voting-consensus",
        "VOTING_PANEL": "general",
        "VOTING_STRATEGY": "consensus"
      }
    }
  }
}
```

## 📋 **Supported Models**

### **OpenRouter Models (2025 Updated)**

#### **🆓 FREE Models (Recommended)**
- `deepseek/deepseek-r1-0528:free` - **NEW** Latest DeepSeek R1 reasoning model (671B params)
- `deepseek/deepseek-r1-0528-qwen3-8b:free` - **NEW** Distilled 8B reasoning model
- `mistralai/devstral-small:free` - **NEW** 24B coding-focused model (SWE-Bench optimized)
- `sarvamai/sarvam-m:free` - **NEW** Multilingual model with reasoning (24B params)
- `google/gemma-3n-e4b-it:free` - **NEW** Google's latest Gemma model
- `meta-llama/llama-3.3-8b-instruct:free` - **UPDATED** Meta's latest Llama
- `microsoft/phi-4-reasoning:free` - **NEW** Microsoft's reasoning model
- `microsoft/phi-4-reasoning-plus:free` - **NEW** Enhanced reasoning model
- `qwen/qwen3-8b:free` - **NEW** Qwen3 8B model
- `qwen/qwen3-14b:free` - **NEW** Qwen3 14B model
- `qwen/qwen3-30b-a3b:free` - **NEW** Qwen3 30B model
- `qwen/qwen3-32b:free` - **NEW** Qwen3 32B model
- `thudm/glm-z1-32b:free` - **NEW** GLM reasoning model (32B params)

#### **💎 Premium Models**
- `anthropic/claude-opus-4` - **NEW** Most powerful Claude model (2025)
- `anthropic/claude-sonnet-4` - **NEW** High performance Claude (2025)
- `google/gemini-2.5-pro-preview` - **NEW** Google's latest Gemini Pro
- `google/gemini-2.5-flash-preview-05-20` - **NEW** Fast Gemini model
- `openai/gpt-4o` - OpenAI's flagship model
- `openai/gpt-4o-mini` - Compact and powerful
- `openai/o1-preview` - **NEW** OpenAI's reasoning model
- `openai/o1-mini` - **NEW** Compact reasoning model
- `anthropic/claude-3-5-sonnet-20241022` - Recommended balance
- `anthropic/claude-3-5-haiku-20241022` - Fastest Claude
- `deepseek/deepseek-chat` - General purpose (DeepSeek-V3)
- `deepseek/deepseek-reasoner` - **NEW** Advanced reasoning (DeepSeek-R1)

### **Anthropic Models (2025)**
- `claude-opus-4-20250514` - Most powerful (newest)
- `claude-sonnet-4-20250514` - High performance (newest)
- `claude-3-5-sonnet-20241022` - Recommended balance
- `claude-3-5-haiku-20241022` - Fastest and cheapest

**Note**: Anthropic models are also available through OpenRouter with the following IDs:
- `anthropic/claude-opus-4` - Claude Opus 4 via OpenRouter
- `anthropic/claude-sonnet-4` - Claude Sonnet 4 via OpenRouter
- `anthropic/claude-3-5-sonnet-20241022` - Claude 3.5 Sonnet via OpenRouter
- `anthropic/claude-3-5-haiku-20241022` - Claude 3.5 Haiku via OpenRouter

### **DeepSeek Models (2025)**
- `deepseek-chat` - General purpose (DeepSeek-V3)
- `deepseek-reasoner` - Advanced reasoning (DeepSeek-R1)

**Note**: DeepSeek models are also available FREE through OpenRouter:
- `deepseek/deepseek-r1-0528:free` - **FREE** Latest R1 reasoning model (671B params)
- `deepseek/deepseek-r1-0528-qwen3-8b:free` - **FREE** Distilled 8B version
- `deepseek/deepseek-chat` - General purpose via OpenRouter (paid)
- `deepseek/deepseek-reasoner` - Advanced reasoning via OpenRouter (paid)

### **Google Gemini Models (2025 - Confirmed Working)**
- `gemini-2.5-flash-preview-05-20` - **LATEST** Most advanced multimodal model (May 2025)
- `gemini-2.0-flash` - **STABLE** Next-gen features with enhanced speed
- `gemini-2.0-flash-001` - **STABLE** Versioned 2.0 Flash model
- `gemini-2.0-flash-lite` - **FAST** Optimized for speed and cost efficiency
- `gemini-1.5-flash-latest` - **RELIABLE** Fast and versatile multimodal
- `gemini-1.5-flash-8b-latest` - **LIGHTWEIGHT** Efficient 8B parameter model
- `gemini-1.5-flash` - **PRODUCTION** Stable Flash model
- `gemini-1.5-flash-8b` - **EFFICIENT** Stable 8B model

**Experimental Models** (May have rate limits):
- `gemini-2.5-pro-preview-06-05` - **PREVIEW** Most powerful reasoning model
- `gemini-2.0-flash-thinking-exp-01-21` - **EXPERIMENTAL** Advanced thinking model
- `gemini-2.0-flash-exp` - **EXPERIMENTAL** Latest experimental features

**Note**: All models tested and confirmed working with the provided API key. Gemini models support multimodal inputs (text, images, audio, video) and provide excellent performance for various tasks.

## 🆕 **What's New in 2025**

### **🚀 Latest Model Updates**
- **13 FREE models** now available through OpenRouter
- **4 CONFIRMED Gemini models** tested and working (2025)
- **DeepSeek R1 0528**: Latest reasoning model with 671B parameters
- **Gemini 2.5 Flash Preview**: Google's most advanced multimodal model
- **Mistral Devstral Small**: 24B coding-focused model optimized for SWE-Bench
- **Microsoft Phi-4**: New reasoning models with enhanced capabilities
- **Qwen3 Series**: Multiple variants (8B, 14B, 30B, 32B) all available for free
- **Anthropic Claude 4**: Opus and Sonnet variants now available
- **Google Gemini 2.0 Flash**: Next-generation features with enhanced speed

### **🔧 Enhanced Features**
- **🗳️ Multi-Model AI Voting**: Multiple AI models vote on best responses
- **🤖 AI Agent Panels**: Specialized agent groups (coding, reasoning, general, gemini)
- **📊 Consensus Algorithms**: Multiple voting strategies (majority, consensus, weighted)
- **🎯 Smart Agent Selection**: Performance-based agent selection
- **🌐 Multi-Provider Support**: OpenRouter + Google Gemini + DeepSeek + Anthropic
- **Automatic Model Failover**: Seamlessly switches between providers
- **Smart API Key Rotation**: Supports multiple keys per provider
- **Enhanced Error Handling**: Better recovery from API failures
- **Real-time Status Monitoring**: Track provider health and usage
- **Improved Data Collection**: Better quality filtering for AI training

## 🛠️ **Installation**

### **VSCode MCP Configuration**

1. **Open VSCode Settings** (Ctrl/Cmd + ,)
2. **Search for "MCP"** or go to Extensions → MCP
3. **Add the configuration** above to your MCP settings
4. **Restart VSCode** to activate

### **Alternative: Direct Installation**
```bash
# Install globally
npm install -g zai-mcp-server

# Or run directly
npx zai-mcp-server@latest
```

## 🎯 **Available Tools**

### **🔄 AI-to-AI Loop Tools**
- `activate_infinite_loop` - Start AI-to-AI improvement loops
- `stop_ai_loops` - Stop all active loops
- `list_active_loops` - View running loops
- `get_ai_prompts` - Get AI-generated prompts
- `acknowledge_agent_response` - Process AI responses

### **🗳️ Multi-Model Voting Tools**
- `ai_voting_request` - Submit prompt for multi-model AI consensus
- `get_voting_history` - View recent voting sessions
- `get_agent_performance` - Check AI agent performance stats

### **🤖 Provider Management Tools**
- `get_ai_provider_status` - Check provider status
- `reset_ai_providers` - Reset failed providers

## 🗳️ **AI Voting System**

### **How It Works**
The ZAI MCP Server features an advanced **multi-model voting system** where multiple AI agents collaborate to provide the best possible responses:

1. **🤖 Agent Selection**: System selects specialized AI agents based on the task
2. **📝 Response Generation**: Each agent generates their own response
3. **🗳️ Voting Phase**: All agents vote on which response is best
4. **🎯 Consensus**: System calculates consensus and selects winner
5. **📊 Learning**: Agent performance is tracked and improved over time

### **Voting Panels**

#### **🔧 General Panel** (Default)
- **DeepSeek R1**: Reasoning specialist (671B params)
- **Mistral Devstral**: Coding expert (24B params)
- **Microsoft Phi-4**: Analysis agent
- **Qwen3 14B**: General assistant
- **Llama 3.3**: Conversation expert

#### **💻 Coding Panel**
- **Mistral Devstral**: Lead coding specialist
- **DeepSeek R1 Qwen**: Reasoning + coding
- **Microsoft Phi-4+**: Development expert
- **Qwen3 32B**: Large model for complex projects

#### **🧠 Reasoning Panel**
- **DeepSeek R1**: State-of-the-art reasoning
- **Microsoft Phi-4**: Analytical thinking
- **GLM Z1**: Creative reasoning
- **Qwen3 30B**: Data analysis

#### **💎 Premium Panel** (Requires Paid APIs)
- **Claude Opus 4**: Most powerful model
- **OpenAI o1**: Advanced reasoning
- **Gemini 2.5 Pro**: Multimodal capabilities
- **Claude Sonnet 4**: High performance

### **Voting Strategies**

- **🗳️ Majority**: Simple majority wins (50%+ threshold)
- **🤝 Consensus**: Strong agreement required (70%+ threshold)
- **⚖️ Weighted**: Votes weighted by agent expertise and confidence
- **💯 Unanimous**: All agents must agree (100% threshold)

### **Example Usage**

```javascript
// Request AI voting on a coding problem
await ai_voting_request({
  prompt: "Optimize this React component for performance",
  panel: "coding",
  strategy: "consensus",
  maxAgents: 4
});

// Get voting history
await get_voting_history({ limit: 5 });

// Check agent performance
await get_agent_performance();
```

## 💡 **Usage Examples**

### **Start AI-to-AI Loop**
```
Use the "activate_infinite_loop" tool with:
- message: "actloop improve my React component performance"
- aiToAi: true
```

### **Check Provider Status**
```
Use the "get_ai_provider_status" tool to see:
- Current provider and model
- Available API keys
- Failed providers
- Request statistics
```

### **Stop Loops**
```
Use "stop_ai_loops" with:
- message: "stploop"
```

## 📊 **AI Model Development Contribution**

**Important Notice**: By using the ZAI MCP Server, you acknowledge and agree that AI-to-AI interactions facilitated by this server may be utilized for AI model development, research, and improvement initiatives. This contributes to the advancement of artificial intelligence technology and helps create better AI systems for the community.

### **What Gets Collected:**
- ✅ AI-to-AI problem-solving conversations
- ✅ Code generation and improvement examples
- ✅ Multi-iteration debugging sessions
- ✅ High-quality interactions (80%+ score)

### **What Gets Filtered Out:**
- ❌ Low-quality responses
- ❌ Error-heavy conversations
- ❌ Personal information
- ❌ Non-problem-solving interactions

### **Data Usage:**
- Training data is used to improve AI models
- Helps advance AI-to-AI collaboration research
- Contributes to open AI development
- All usage complies with applicable data protection regulations

## 🔧 **Configuration Options**

### **Environment Variables**
- `OPENROUTER_API_KEY` - Comma-separated OpenRouter keys
- `ANTHROPIC_API_KEY` - Comma-separated Anthropic keys
- `DEEPSEEK_API_KEY` - Comma-separated DeepSeek keys
- `MODEL` - Primary model to use
- `ZAI_FREE_MODE` - Always true (no license needed)
- `ZAI_DATA_COLLECTION` - Always true (automatic)

### **Multiple API Keys**
```json
"OPENROUTER_API_KEY": "key1,key2,key3,key4"
```
The server automatically rotates between keys for high availability.

## 🚀 **Advanced Features**

### **Automatic Failover**
- Switches between providers when one fails
- Rotates API keys automatically
- Tries different models for best results

### **Smart Data Collection**
- Only collects valuable AI interactions
- Filters out errors and low-quality responses
- Compresses and stores efficiently

### **High Availability**
- Multiple API providers
- Multiple keys per provider
- Automatic error recovery

## 🆓 **Why It's Free**

This MCP server is completely free because:
- **No License Validation** - No restrictions or paywalls
- **Community Driven** - Open source development
- **Data Collection** - Valuable training data helps fund development
- **AI Advancement** - Contributes to AI research and development

## 📊 **Data Collection**

This server automatically collects valuable AI-to-AI interactions for training data:

### **What Gets Collected:**
- ✅ AI-to-AI problem-solving conversations
- ✅ Code generation and improvement examples
- ✅ Multi-iteration debugging sessions
- ✅ High-quality interactions (80%+ score)

### **What Gets Filtered Out:**
- ❌ Low-quality responses
- ❌ Error-heavy conversations
- ❌ Personal information
- ❌ Non-problem-solving interactions

### **Data Usage:**
- Training data is used to improve AI models
- Helps advance AI-to-AI collaboration research
- Contributes to open AI development

## 🔧 **Configuration Options**

### **Environment Variables**
- `OPENROUTER_API_KEY` - Comma-separated OpenRouter keys
- `ANTHROPIC_API_KEY` - Comma-separated Anthropic keys
- `DEEPSEEK_API_KEY` - Comma-separated DeepSeek keys
- `MODEL` - Primary model to use
- `ZAI_FREE_MODE` - Always true (no license needed)
- `ZAI_DATA_COLLECTION` - Always true (automatic)

### **Multiple API Keys**
```json
"OPENROUTER_API_KEY": "key1,key2,key3,key4"
```
The server automatically rotates between keys for high availability.

## 🚀 **Advanced Features**

### **Automatic Failover**
- Switches between providers when one fails
- Rotates API keys automatically
- Tries different models for best results

### **Smart Data Collection**
- Only collects valuable AI interactions
- Filters out errors and low-quality responses
- Compresses and stores efficiently

### **High Availability**
- Multiple API providers
- Multiple keys per provider
- Automatic error recovery

## 🆓 **Why It's Free**

This MCP server is completely free because:
- **No License Validation** - No restrictions or paywalls
- **Community Driven** - Open source development
- **Data Collection** - Valuable training data helps fund development
- **AI Advancement** - Contributes to AI research and development

## 🤝 **Contributing**

We welcome contributions! This project helps advance AI-to-AI collaboration research.

## 📄 **License**

MIT License - Use freely in any project, commercial or personal.

## 🔗 **Links**



- **NPM**: [zai-mcp-server](https://www.npmjs.com/package/zai-mcp-server)

---

**🎉 Start using your FREE multi-provider AI MCP server today!**
