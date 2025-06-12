# Huddle IPFS Node Manager

A simple, user-friendly tool for setting up and managing persistent IPFS nodes without relying on paid services.

## Installation Options

### Option 1: Install via IPFS (Self-hosting in action!)

The easiest way to install Huddle IPFS Node Manager is directly from IPFS itself:

```bash
# For macOS/Linux
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash

# Or if you prefer to review before executing
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh -o install-huddle-ipfs.sh
chmod +x install-huddle-ipfs.sh
./install-huddle-ipfs.sh
```

This method bootstraps the installation from IPFS itself, demonstrating the power of the technology you're about to use!

### Option 2: Install via Homebrew (macOS/Linux)

If you prefer using package managers:

```bash
# Add the Huddle tap
brew tap huddle/ipfs

# Install the formula
brew install ipfs-node-manager
```

## Quick Start

### Option 1: Install via IPFS (Recommended)

```bash
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash
```

### Option 2: After installation, set up your IPFS node

```bash
# Start the setup process
ipfs-setup

# Once complete, check your node status
~/ipfs-helper.sh status
```

## Enterprise Features

### Version Management

Check your installed version and check for updates:

```bash
ipfs-manager-version
```

### Silent Installation for Deployment

For automated deployment across multiple systems:

```bash
# Silent installation (no prompts)
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash -s -- --silent

# Force reinstallation/upgrade
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash -s -- --force

# Combine options
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash -s -- --silent --force
```

### Configuration Management

When upgrading, your configuration is automatically backed up before any changes are made. Previous configuration files are stored in timestamped backup directories.

### Uninstallation

To remove the software:

```bash
ipfs-manager-uninstall
```

## Features

- **Zero-subscription costs**: Host your own IPFS infrastructure
- **Persistence**: Automatic configuration for always-on pinning
- **Easy content management**: Simple tools for adding and managing content
- **Web management API**: Optional API for remote management
- **Self-contained**: Manages all dependencies and configurations automatically
- **Enterprise-ready**: Version control, silent installation, and configuration management

## About

HuddleAI Co. builds tools that make decentralized technologies accessible to everyone. The IPFS Node Manager empowers individuals and organizations to participate in the decentralized web without relying on third-party services.

## License

MIT 