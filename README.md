# Overview init-env

This Bash script automates the installation of several essential packages and tools on an Ubuntu system, including Docker, SDKMAN (with Java 21), NVM (with Node 21), and VSCode.  
Made by Vinicius Barbosa

## What It Does

- **Useful Packages Installation:**  
  Updates the package list and installs packages like `curl`, `zip`, `unzip`, and `ca-certificates`.

- **Docker Installation:**  
  Uninstalls any existing Docker-related packages, adds the official Docker repository and its GPG key, installs Docker Engine and related components, configures the Docker group, and applies group changes using `newgrp docker` in a subshell.

- **NVM and Node.js Installation:**  
  Downloads and installs NVM, then sets up Node.js (version 22.8.0 is used in the script).

- **SDKMAN and Java Installation:**  
  Downloads and installs SDKMAN, then installs and sets Java version 21.0.2-open as the current version. It also displays the installed Java version.

- **Visual Studio Code Launch:**  
  Opens VSCode with the current directory as the workspace.

## Prerequisites

- A running Ubuntu system.
- Sudo privileges.
- An active internet connection.

## Usage

1. **Make the script executable:**

   ```bash
   sudo bash init-env.sh
