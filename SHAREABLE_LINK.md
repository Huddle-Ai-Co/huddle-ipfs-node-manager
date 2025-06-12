# Huddle IPFS Node Manager - Shareable Links

This document contains everything you need to share the Huddle IPFS Node Manager (by HuddleAI Co.) with users who may not have GitHub or Homebrew access.

## Quick Installation Link

Users can install the Huddle IPFS Node Manager with this simple command:

```bash
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash
```

## Permanent IPNS Link (Always Points to Latest Version)

This link will always point to the latest version:

```bash
curl -L https://ipfs.io/ipns/k51qzi5uqu5di9u60hshlkcr605megfry21dx7zmdbla2jzte7dub3em1e5fd4/install.sh | bash
```

## For Users Who Want to Review Before Installing

Share these instructions for users who prefer to review scripts before executing:

```bash
# Download the installer
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh -o huddle-ipfs-installer.sh

# Make it executable
chmod +x huddle-ipfs-installer.sh

# Review the script (optional)
less huddle-ipfs-installer.sh

# Run when ready
./huddle-ipfs-installer.sh
```

## Enterprise Installation Options

For automated deployment across multiple systems:

```bash
# Silent installation (no prompts)
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash -s -- --silent

# Force reinstallation/upgrade
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash -s -- --force

# Combine options
curl -L https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh | bash -s -- --silent --force
```

## Direct IPFS Gateway Links

Users can browse the entire project contents at:

- **Latest version (IPFS hash):**  
  [https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/](https://ipfs.io/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/)

- **Permanent link (IPNS):**  
  [https://ipfs.io/ipns/k51qzi5uqu5di9u60hshlkcr605megfry21dx7zmdbla2jzte7dub3em1e5fd4/](https://ipfs.io/ipns/k51qzi5uqu5di9u60hshlkcr605megfry21dx7zmdbla2jzte7dub3em1e5fd4/)

## Alternative Gateway Links

In case ipfs.io is blocked or unavailable, users can access the content through any of these alternative public IPFS gateways:

```
https://dweb.link/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh
https://gateway.pinata.cloud/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh
https://cf-ipfs.com/ipfs/QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ/install.sh
```

## For IPFS Users: Pin the Content

If users already have IPFS installed, they can help distribute the content by pinning it:

```bash
ipfs pin add QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ
```

## Making the Content Persistent

The Huddle IPFS Node Manager is currently pinned on:

1. Your local IPFS node
2. Any IPFS nodes that have pinned the content
3. Accessible via IPNS at: `k51qzi5uqu5di9u60hshlkcr605megfry21dx7zmdbla2jzte7dub3em1e5fd4`

For even more persistence, consider:

1. **Using a pinning service** like Pinata or Infura to ensure 24/7 availability
2. **Setting up DNSLink** for easier updates (see IPFS_DISTRIBUTION.md)

## Ensuring Long-term Availability

For maximum persistence without relying on external services, ask several trusted peers to pin the content with:

```bash
ipfs pin add QmbyaB8jqJpoeze6GHEY2oTtbDiFobh52NNznsrfMxVzjQ
```

This distributed approach ensures the content remains available even if some nodes go offline.

## Version Management

Users can check for updates and manage versions with:

```bash
# After installation, check version
ipfs-manager-version

# Uninstall if needed
ipfs-manager-uninstall
``` 