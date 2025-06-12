# ZAI MCP Server

An advanced Model Context Protocol (MCP) server that provides AI-powered infinite loop capabilities for continuous improvement and AI-to-AI communication.

## 🚀 Features

### Core Functionality
- **Infinite Loop System**: Activate continuous AI-powered improvement loops for any topic
- **AI-to-AI Communication**: Enable seamless communication between AI agents
- **Multi-Provider Support**: Integration with OpenRouter, Anthropic, and DeepSeek AI providers
- **Dynamic Loop Management**: Start, stop, monitor, and configure loops in real-time
- **Intelligent Prompt Generation**: AI-generated prompts ready for VSCode AI assistant

### Advanced Capabilities
- **Agent Status Monitoring**: Real-time tracking of agent health and availability
- **API Key Management**: Automatic handling of multiple API keys with rate limiting
- **Model Status Tracking**: Monitor available, failed, and current AI models
- **Session Management**: Clean session state management for different projects
- **Error Recovery**: Automatic retry mechanisms for failed models and API keys

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/Zrald1/zai-mcp-server.git
cd zai-mcp-server

# Install dependencies
npm install

# Configure your AI API keys
cp .env.example .env
# Edit .env with your API keys
```

## 🔧 Configuration

Create a `.env` file with your AI provider API keys:

```env
OPENROUTER_API_KEY=your_openrouter_key
ANTHROPIC_API_KEY=your_anthropic_key
DEEPSEEK_API_KEY=your_deepseek_key
```

## 🎯 Usage

### Starting Infinite Loops

Activate an infinite loop for continuous AI improvement:

```javascript
// AI-to-AI communication mode (default)
activate_infinite_loop("actloop improve code quality")

// Regular loop mode
activate_infinite_loop("actloop optimize performance", { aiToAi: false })
```

### Managing Loops

```javascript
// List all active loops
list_active_loops()

// Get specific loop status
get_loop_status(loopId)

// Stop specific loop
stop_loop(loopId)

// Stop all loops
stop_all_loops()
```

### AI Prompt Management

```javascript
// Get AI-generated prompts
get_ai_prompts({ limit: 5 })

// Acknowledge agent response
acknowledge_agent_response(loopId, "Agent completed the task successfully")
```

## 🛠️ Available Tools

### Loop Management
- `activate_infinite_loop` - Start AI-powered improvement loops
- `stop_loop` - Stop specific loops by ID
- `stop_all_loops` - Stop all active loops
- `list_active_loops` - List currently active loops
- `get_loop_status` - Get detailed loop status
- `update_loop_interval` - Modify loop timing

### AI Provider Management
- `get_ai_provider_status` - Check all AI provider status
- `get_model_status` - Monitor OpenRouter model availability
- `get_api_key_status` - Check API key usage and limits
- `reset_ai_providers` - Reset failed providers
- `reset_failed_models` - Retry failed models

### Agent Communication
- `get_ai_prompts` - Retrieve AI-generated prompts
- `acknowledge_agent_response` - Confirm agent task completion
- `check_agent_status` - Monitor agent availability
- `get_pending_responses` - Check waiting responses

### Session Management
- `reset_session` - Clear all loops and state
- `clear_agent_busy_state` - Emergency state reset

## 🔄 AI-to-AI Loop Workflow

1. **Activation**: Use `actloop [topic]` to start continuous improvement
2. **Processing**: AI agents communicate and iterate on the topic
3. **Monitoring**: Track progress with status tools
4. **Acknowledgment**: Confirm completed tasks to continue the loop
5. **Termination**: Use `stploop` to stop AI-to-AI loops

## 📊 Monitoring & Status

The server provides comprehensive monitoring:

- **Agent Health**: Real-time agent status and availability
- **Loop Performance**: Iteration counts, timing, and success rates
- **API Usage**: Rate limits, failures, and key rotation
- **Model Availability**: Track which AI models are operational

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built for the Model Context Protocol ecosystem
- Designed for seamless AI agent integration
- Optimized for VSCode AI assistant workflows

---

**Made with ❤️ by [Zrald1](https://github.com/Zrald1)**
