# Exe Runner

Exe Runner runs Windows programs and games on Linux. This branch is its apt repository for Ubuntu 24.04 and newer
(amd64), binary packages only. The source code is not public yet.

## Install

Download [exe-runner_0.1.2_amd64.deb](https://simonlinuxcraft.github.io/exe-runner/exe-runner_0.1.2_amd64.deb) and install it:

    sudo apt install ./exe-runner_0.1.2_amd64.deb

The package adds this repository and its key, so updates arrive with the system's other updates.

Or add the repository first and install from it:

    wget -qO- https://simonlinuxcraft.github.io/exe-runner/exe-runner.gpg | sudo tee /usr/share/keyrings/exe-runner.gpg > /dev/null
    printf 'Types: deb\nURIs: https://simonlinuxcraft.github.io/exe-runner\nSuites: ./\nSigned-By: /usr/share/keyrings/exe-runner.gpg\n' | sudo tee /etc/apt/sources.list.d/exe-runner.sources > /dev/null
    sudo apt update
    sudo apt install exe-runner

Signing key: `047D304C3857A10BC4C6319ACB4B04B91587EFCD`
