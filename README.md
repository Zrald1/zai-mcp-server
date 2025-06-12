# ZAI MCP Server

**FREE Multi-Provider AI MCP Server** with support for OpenRouter, Anthropic, and DeepSeek APIs. Features automatic failover, AI-to-AI loops, and smart data collection. No license validation required - completely free for all users!

## ✨ Key Features

🆓 **Completely FREE** - No license validation or restrictions
🤖 **Multi-Provider Support** - OpenRouter, Anthropic, DeepSeek APIs
🔄 **Automatic Failover** - Smart switching between providers/models
🔁 **AI-to-AI Loops** - Infinite improvement cycles
📊 **Smart Data Collection** - Automatic training data collection
⚡ **High Availability** - Multiple API keys with rotation
🎯 **Quality Filtering** - Only valuable interactions collected
🌐 **Global Access** - Works worldwide, no restrictions

## 🚀 Quick Setup

### Option 1: OpenRouter (Recommended - Free Models Available)
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "OPENROUTER_API_KEY": "sk-or-v1-abc123...,sk-or-v1-def456...,sk-or-v1-ghi789...",
        "MODEL": "google/gemini-2.0-flash-exp:free"
      }
    }
  }
}
```

### Option 2: Anthropic Claude
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

### Option 3: DeepSeek (Best Value)
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

### Option 4: Multi-Provider (Ultimate Setup)
```json
{
  "mcpServers": {
    "zai-mcp-server": {
      "command": "npx",
      "args": ["-y", "zai-mcp-server@latest"],
      "env": {
        "OPENROUTER_API_KEY": "sk-or-v1-abc123...,sk-or-v1-def456...",
        "ANTHROPIC_API_KEY": "sk-ant-api03-abc123...",
        "DEEPSEEK_API_KEY": "sk-abc123...",
        "MODEL": "deepseek-chat"
      }
    }
  }
}
```

## 📋 Supported Models

### OpenRouter Models
- `google/gemini-2.0-flash-exp:free` - **FREE** (Recommended)
- `anthropic/claude-3-haiku:beta` - Fast and efficient
- `openai/gpt-4o-mini` - Compact and powerful
- `meta-llama/llama-3.1-8b-instruct:free` - **FREE** Open source
- `qwen/qwen-2.5-72b-instruct` - High performance

### Anthropic Models (2025)
- `claude-opus-4-20250514` - Most powerful (newest)
- `claude-sonnet-4-20250514` - High performance (newest)
- `claude-3-5-sonnet-20241022` - Recommended balance
- `claude-3-5-haiku-20241022` - Fastest and cheapest

### DeepSeek Models (2025)
- `deepseek-chat` - General purpose (DeepSeek-V3)
- `deepseek-reasoner` - Advanced reasoning (DeepSeek-R1)

## 🛠️ Installation

### VSCode MCP Configuration
1. Open VSCode Settings (Ctrl/Cmd + ,)
2. Search for "MCP" or go to Extensions → MCP
3. Add the configuration above to your MCP settings
4. Restart VSCode to activate

### Alternative: Direct Installation
```bash
# Install globally
npm install -g zai-mcp-server

# Or run directly
npx zai-mcp-server@latest
```

## 🎯 Available Tools

- `activate_infinite_loop` - Start AI-to-AI improvement loops
- `stop_ai_loops` - Stop all active loops
- `list_active_loops` - View running loops
- `get_ai_provider_status` - Check provider status
- `reset_ai_providers` - Reset failed providers
- `get_ai_prompts` - Get AI-generated prompts
- `acknowledge_agent_response` - Process AI responses

## 💡 Usage Examples

### Start AI-to-AI Loop
Use the "activate_infinite_loop" tool with:
- **message**: `"actloop improve my React component performance"`
- **aiToAi**: `true`

### Check Provider Status
Use the "get_ai_provider_status" tool to see:
- Current provider and model
- Available API keys
- Failed providers
- Request statistics

### Stop Loops
Use "stop_ai_loops" with:
- **message**: `"stploop"`

## 📊 Data Collection

This server automatically collects valuable AI-to-AI interactions for training data:

### What Gets Collected:
✅ AI-to-AI problem-solving conversations
✅ Code generation and improvement examples
✅ Multi-iteration debugging sessions
✅ High-quality interactions (80%+ score)

### What Gets Filtered Out:
❌ Low-quality responses
❌ Error-heavy conversations
❌ Personal information
❌ Non-problem-solving interactions

### Data Usage:
- Training data is used to improve AI models
- Helps advance AI-to-AI collaboration research
- Contributes to open AI development

## 🔧 Configuration Options

### Environment Variables
- `OPENROUTER_API_KEY` - Comma-separated OpenRouter keys
- `ANTHROPIC_API_KEY` - Comma-separated Anthropic keys
- `DEEPSEEK_API_KEY` - Comma-separated DeepSeek keys
- `MODEL` - Primary model to use
- `ZAI_FREE_MODE` - Always true (no license needed)
- `ZAI_DATA_COLLECTION` - Always true (automatic)

### Multiple API Keys
```json
"OPENROUTER_API_KEY": "key1,key2,key3,key4"
```
The server automatically rotates between keys for high availability.

## 🚀 Advanced Features

### Automatic Failover
- Switches between providers when one fails
- Rotates API keys automatically
- Tries different models for best results

### Smart Data Collection
- Only collects valuable AI interactions
- Filters out errors and low-quality responses
- Compresses and stores efficiently

### High Availability
- Multiple API providers
- Multiple keys per provider
- Automatic error recovery

## 🆓 Why It's Free

This MCP server is completely free because:

- **No License Validation** - No restrictions or paywalls
- **Community Driven** - Open source development
- **Data Collection** - Valuable training data helps fund development
- **AI Advancement** - Contributes to AI research and development

## 🤝 Contributing

We welcome contributions! This project helps advance AI-to-AI collaboration research.

## 📄 License

MIT License - Use freely in any project, commercial or personal.

## 🔗 Links

- **GitHub**: [https://github.com/Zrald1/zai-mcp-server.git](https://github.com/Zrald1/zai-mcp-server.git)
- **NPM**: [zai-mcp-server](https://www.npmjs.com/package/zai-mcp-server)
- **Issues**: [Report bugs](https://github.com/Zrald1/zai-mcp-server/issues)

---

**Made with ❤️ by [zraldloop](https://github.com/Zrald1)**
