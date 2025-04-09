# Configure GPG Keys for Verified GitHub Commits

This guide provides a straightforward way to set up GPG keys to sign your Git commits, resulting in a "Verified" badge on GitHub. Verified commits provide assurance that the commit genuinely comes from you.

## Why Verified Commits?

- **Trust:** Shows others that the commits haven't been tampered with and originate from a verified source.
- **Authenticity:** Helps prevent impersonation in commit authorship.
- **Professionalism:** Often required or encouraged in open-source projects and professional environments.

## Prerequisites

1.  **Git:** Installed on your system. ([Download Git](https://git-scm.com/downloads))
2.  **GPG:** GnuPG (GNU Privacy Guard) command-line tools installed.
    - **macOS:** Often pre-installed. If not, use Homebrew: `brew install gnupg`
    - **Linux (Debian/Ubuntu):** `sudo apt update && sudo apt install gnupg`
    - **Linux (Fedora):** `sudo dnf install gnupg2`
    - **Windows:** Install [Gpg4win](https://www.gpg4win.org/) (which includes GnuPG) or use Git Bash which often comes with a version of GPG.

## Steps

### 1. Check for Existing GPG Keys

First, check if you already have a GPG key pair suitable for signing.

```bash
gpg --list-secret-keys --keyid-format=long
```
