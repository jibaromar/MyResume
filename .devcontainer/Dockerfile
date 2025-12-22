# .devcontainer/Dockerfile
FROM texlive/texlive:latest-small

# Set noninteractive frontend
ENV DEBIAN_FRONTEND=noninteractive

# Install basic utilities
RUN apt-get update && apt-get install -y \
    curl \
    wget \
    git \
    openssh-client \
    build-essential \
    python3 \
    python3-pip \
    texlive-xetex \
    texlive-latex-recommended \
    texlive-latex-extra \
    texlive-fonts-recommended \
    texlive-fonts-extra \
    biber \
    unzip \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /workspace
