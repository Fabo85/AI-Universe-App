# AI Universe - Desktop Platform

A comprehensive AI ecosystem with 9 specialized modules for productivity, creativity, and learning.

## Features

- **Personal AI Assistant**: Intelligent task management with persistent memory
- **Creative AI Suite**: Art, music, video, and content generation
- **AI Learning Mentor**: Personalized learning paths and skill development
- **Code GPT**: Advanced coding assistance with Monaco Editor
- **Eidolon Scribe**: Transform daily logs into mythical narratives
- **Flow Architect**: Custom ambient soundscapes
- **Gost@Termux**: Hacker companion for terminal access
- **Code Mate**: Deploy & optimize code with AI assistance
- **Novel Writer**: AI-powered story creation

## API Configuration

### OpenAI API Key vs GitHub Token

**Question**: Is it possible for OpenAI API key to be replaced with GitHub token?

**Answer**: No, OpenAI API keys and GitHub tokens serve different purposes and cannot be directly replaced:

1. **OpenAI API Key**: Used to authenticate with OpenAI's services (GPT models, DALL-E, etc.)
   - Required for: Chat completions, text generation, image generation
   - Format: `sk-...` (starts with "sk-")
   - Obtained from: https://platform.openai.com/api-keys

2. **GitHub Token**: Used to authenticate with GitHub's API
   - Required for: Repository access, GitHub Actions, code management
   - Format: `ghp_...` or `github_pat_...`
   - Obtained from: GitHub Settings > Developer settings > Personal access tokens

### Alternative Solutions

If you want to avoid using OpenAI API directly, consider these alternatives:

1. **Use GitHub Copilot API** (if available) for code-related features
2. **Implement a backend proxy** that handles API keys securely
3. **Use other AI providers** like Anthropic Claude, Google Gemini, or local models
4. **Create a hybrid approach** using GitHub for code features and OpenAI for general chat

### Current Implementation

The website currently supports:
- OpenAI API key configuration in settings
- Local storage of API keys (client-side only)
- Multiple AI model selection (GPT-4, GPT-4 Turbo, GPT-3.5 Turbo)
- Conversation history and memory sharing between modules

## Setup Instructions

1. Open `index.html` in a web browser
2. Click the Settings button in the top-right corner
3. Enter your OpenAI API key in the AI Configuration section
4. Customize your preferences and save settings
5. Start using the AI modules from the sidebar

## Security Notes

- API keys are stored locally in browser localStorage
- Keys are never sent to external servers (except OpenAI for API calls)
- Consider implementing a backend service for production use
- Use environment variables or secure key management in production

## Development

The website is built with:
- Pure HTML/CSS/JavaScript
- TailwindCSS for styling
- Monaco Editor for code editing
- Font Awesome icons
- Ethers.js for Web3 integration (optional)

No build process required - simply open `index.html` in a browser.

