
# Swift Meadow

Personal academic website built with the **Swift Meadow** template from [HugoBlox](https://hugoblox.com/). The content below is a concise guide for getting the site running locally on macOS. For more detail, see `Install.md`.

## Requirements
- macOS with [Homebrew](https://brew.sh)
- Git

## Setup
```bash
git clone https://github.com/<your-username>/swift-meadow.git
cd swift-meadow

brew install hugo         # Hugo Extended
brew install node         # Node.js + npm
brew install go           # Required for Hugo modules

npm install -g corepack   # Provides pnpm
corepack enable
pnpm -v                   # Downloads pnpm shim on first run

pnpm install              # Install project dependencies
```

## Local Development
```bash
hugo server --bind 0.0.0.0 --baseURL http://localhost:1313 --disableFastRender
```

Open http://localhost:1313/ in your browser and stop the server with `Ctrl+C` when finished.

## Credits
Template: [Swift Meadow](https://hugoblox.com/templates/) by HugoBlox.
