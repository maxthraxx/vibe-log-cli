
<div align="center">

<img width="628" height="176" alt="image" src="https://github.com/user-attachments/assets/1e468c1f-8228-46ad-a441-1b0926edfbc9" />

<p></p>
<h3> Track your building journey with Vibe-Log - the CLI tool that helps developers improve, analyze productivity patterns,  maintain coding streaks, and build in public with AI-powered insights </h3>
<p></p>

<a href="https://vibe-log.dev">
  <img src="https://img.shields.io/badge/by-vibe--log.dev-16A34A" alt="by vibe-log.dev"></a>
  <a href="https://www.npmjs.com/package/vibe-log-cli"><img src="https://img.shields.io/npm/v/vibe-log-cli.svg" alt="npm version"></a>
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT"></a>
  <a href="https://nodejs.org"><img src="https://img.shields.io/node/v/vibe-log-cli.svg" alt="Node.js Version"></a>
  <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
<a href="https://github.com/vibe-log/vibe-log-cli/actions/workflows/tests.yml"><img src="https://github.com/vibe-log/vibe-log-cli/actions/workflows/tests.yml/badge.svg" alt="Tests"></a>
<a href="SECURITY.md"><img src="https://img.shields.io/badge/Security-Policy-blue.svg" alt="Security Policy"></a>
  <a href="https://github.com/vibe-log/vibe-log-cli">
  <img src="https://img.shields.io/badge/⭐_Star-this_repo-22C55E?labelColor=000000" alt="Star this repo">
</a>
  
</p>


[Website](https://vibe-log.dev) • [Report Bug](https://github.com/vibe-log/vibe-log-cli/issues) • [Request Feature](https://github.com/vibe-log/vibe-log-cli/issues)
</div>

![vibe-log](https://github.com/user-attachments/assets/6977e0fb-f02c-4e9c-977f-fe07cc8ba441)

<dib align=left> <h2>🎯 What is Vibe-Log?</h2>
<p></p>
vibe-log is a comprehensive CLI tool that analyzes your coding sessions to extract productivity metrics, emotional insights, and generates engaging Build in Public content. It integrates seamlessly with Claude Code and other AI coding assistants to help you understand your development patterns and share your journey.<p></p>
✨ Key Features

📊 Productivity Analytics - Track goals, code acceptance rates, and session efficiency<br>
📝 Tailored Prompt Engineering Feedback - Improve your AI interaction efficiency<br>
📈 AI Metrics Tracking - Monitor how effectively you're using AI coding assistants<br>
🔥 Vibe Coding Streaks - Keep your momentum alive! Track daily coding streaks with visual flame indicators and maintain consistency<br>
🐦 Build in Public Automation - Draft authentic tweets based on your vibe-coding sessions<br>


</div>

## Quick Start

**Get started with the interactive menu:**
   ```bash
   npx vibe-log-cli
   ```

## Configuration

Configuration is stored in `~/.vibe-log/`


## Supported Coding Engines 

Currently supported:
- ✅ Claude Code

Future:
- 🔜 Cursor
- 🔜 VS Code

## Privacy & Security

### Security Features
- **Secure Token Storage**: Authentication tokens are encrypted using AES-256-GCM with random keys
- **Input Validation**: All user inputs are validated to prevent injection attacks
- **CSRF Protection**: Browser authentication uses CSRF tokens to prevent cross-site attacks
- **Rate Limiting**: Built-in rate limiting to prevent brute force attempts
- **HTTPS Only**: All API communications are restricted to HTTPS
- **Session Security**: Cryptographically secure session IDs (256-bit)
- **Data Sanitization**: All data is sanitized before logging or transmission

### Security Best Practices
- Never share your authentication token
- Keep the CLI updated for the latest security patches 


### Privacy
- **Context-Preserving Sanitization**: Messages are sanitized to remove sensitive data while preserving context
- **What gets redacted/removed**:
  - Code blocks → `[CODE_BLOCK_1: javascript]`
  - API keys/tokens → `[CREDENTIAL_1]`
  - File paths → `[PATH_1]`
  - URLs → `[DATABASE_URL]`, `[API_URL]`
  - Emails → `[EMAIL_1]`
  - Environment variables → `[ENV_VAR_1]`
  - Also Removed: Images/Binary files 
- **What's preserved**: Conversation flow, questions, explanations
- **Transparent**: Preview sanitized data with the interactive prompt
- **Open source**: Review our sanitization at [src/lib/message-sanitizer-v2.ts](src/lib/message-sanitizer-v2.ts)

## Troubleshooting

### Authentication Issues
Try the following: 
- Log out from the CLI
- Clear cookies
- Re-authenticate via the CLI 

### No Sessions Found
- Make sure Claude Code is installed
- Check that you've used Claude Code recently


### Debug Mode
```bash
# Enable debug logging
VIBELOG_DEBUG=1 npx vibe-log-cli send
```

## Contributing

We love your input! We want to make contributing to Vibe-Log CLI as easy and transparent as possible. Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### Quick Start for Contributors

```bash
# Clone the repository
git clone https://github.com/vibe-log/vibe-log-cli.git
cd vibe-log-cli

# Install dependencies
npm install

# Run tests
npm test

# Build the project
npm run build
```

Check out our [open issues](https://github.com/vibe-log/vibe-log-cli/issues) for a list of proposed features and known issues.

## Community

- **GitHub**: Star us on [GitHub](https://github.com/vibe-log/vibe-log-cli)
- **Issues**: Report bugs and request features in [GitHub Issues](https://github.com/vibe-log/vibe-log-cli/issues)
- **Website**: Visit [vibe-log.dev](https://vibe-log.dev)

## Support

Need help? Here are some ways to get support:

- 📖 Read the [documentation](https://vibe-log.dev/docs)
- 🐛 Report bugs in [GitHub Issues](https://github.com/vibe-log/vibe-log-cli/issues)
- 📧 Email us at support@vibe-log.dev

## License

MIT © Vibelog - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Built with love by the Vibe-Log team and our amazing contributors.
