FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# 安装基础工具
RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    gcc \
    make \
    qemu-system-x86 \
    qemu-utils \
    libglib2.0-dev \
    libfdt-dev \
    libpixman-1-dev \
    python3 \
    python3-pip \
    libssl-dev \
    wget \
    curl \
    && rm -rf /var/lib/apt/lists/*

# 设置工作目录
WORKDIR /workspace

# 创建非root用户（Codespaces默认使用vscode用户）
USER vscode
