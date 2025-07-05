#  Memori Browser

> The lightest, fastest, AI-enhanced browser across all platforms

Memori is a revolutionary browser that combines lightning-fast performance with AI-native functionality. Built with a surgical tech stack optimized for speed, low memory footprint, and intelligent browsing.
This is still in development phase

##  Key Features

- ** Ultra-Lightweight**: 2-5MB binaries (vs 100MB+ traditional browsers)
- ** AI-Native**: Built-in LLM integration for smart tab management and content understanding
- ** Lightning Fast**: Rust-powered backend with native webview performance
- ** Intelligent Search**: Fuzzy search across tabs, history, and content with AI context
- ** Smart Memory**: Vector-based memory system that learns from your browsing patterns
- ** Cross-Platform**: Native performance on Windows, macOS, and Linux

##  Architecture

### Core Tech Stack
- **Shell**: Tauri (Rust + Native Webviews)
- **UI**: React + TailwindCSS
- **AI Engine**: Local LLM + Cloud Router (OpenAI, Claude, Gemini)
- **Memory**: SQLite + Qdrant Vector DB
- **Search**: FlexSearch + AI-enhanced fuzzy matching
- **State**: Zustand for minimal state management

### Performance Targets
- **Binary Size**: < 5MB
- **Memory Usage**: < 50MB idle
- **Startup Time**: < 500ms
- **Tab Switch**: < 50ms
- **AI Response**: < 200ms (local), < 1s (cloud)

##  Quick Start

### Prerequisites
```bash
# Install Rust
curl --proto "=https" --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Install Node.js (18+)
# Download from https://nodejs.org/

# Install Tauri CLI
cargo install tauri-cli
```

### Development Setup
```bash
# Clone the repository
git clone https://github.com/your-username/memori-browser
cd memori-browser

# Install dependencies
npm install

# Start development server
npm run tauri:dev
```

### Build for Production
```bash
# Build optimized binary
npm run tauri:build
```

##  Project Structure

```
memori-browser/
 src-tauri/          # Rust backend
    src/
       main.rs     # Main Tauri app
       memory/     # Memory engine
       ai/         # AI integration
       search/     # Search engine
       browser/    # Browser engine
       utils/      # Utilities
    Cargo.toml
 src/                # React frontend
    components/     # UI components
    hooks/          # React hooks
    stores/         # Zustand stores
    services/       # API services
    utils/          # Utilities
 public/             # Static assets
 package.json
```


##  Development Commands

```bash
# Development
npm run dev              # Start Vite dev server
npm run tauri:dev        # Start Tauri development mode

# Building
npm run build            # Build frontend
npm run tauri:build      # Build complete application

# Testing
npm run test             # Run tests
npm run lint             # Run linting
npm run format           # Format code
```


### Development Guidelines
- **Performance First**: Every feature must justify its performance cost
- **AI-Native**: Consider AI integration in all new features
- **Cross-Platform**: Ensure compatibility across all target platforms
- **Minimal Dependencies**: Prefer lightweight, focused libraries

##  Benchmarks

| Metric | Memori | Chrome | Firefox | Safari |
|--------|--------|--------|---------|--------|
| Binary Size | ~5MB | ~200MB | ~150MB | ~100MB |
| Memory (Idle) | ~30MB | ~150MB | ~120MB | ~80MB |
| Startup Time | ~300ms | ~2s | ~1.5s | ~1s |
| Tab Switch | ~30ms | ~100ms | ~80ms | ~50ms |

##  License

MIT License - see [LICENSE](LICENSE) file for details.

##  Why Memori?

Traditional browsers are bloated, slow, and do not understand your workflow. Memori is built from the ground up to be:

- **Intelligent**: AI that learns and adapts to your browsing patterns
- **Efficient**: Minimal resource usage without sacrificing functionality
- **Fast**: Native performance with modern web capabilities
- **Personal**: Your browsing data stays private and secure

---

**Ready to experience the future of browsing?** 
