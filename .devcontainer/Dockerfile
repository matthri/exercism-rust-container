# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.217.4/containers/rust/.devcontainer/base.Dockerfile

# [Choice] Debian OS version (use bullseye on local arm64/Apple Silicon): buster, bullseye
ARG VARIANT="bullseye"
FROM mcr.microsoft.com/vscode/devcontainers/rust:0-${VARIANT}

RUN curl -s https://api.github.com/repos/exercism/cli/releases/latest | \
    grep -E 'browser_download_url' | \
    grep linux-$(uname -m) | \
    cut -d '"' -f 4 | \ 
    wget -qi - -O - | \
    tar -xz -C /usr/local/bin exercism

# [Optional] Uncomment this section to install additional packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>
