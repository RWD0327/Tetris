# Dockerfile
FROM archlinux:latest

# Install necessary packages
RUN pacman -Syu --noconfirm \
    gcc \
    make \
    nano \
    qemu \
    nasm \
    glfw \
    && pacman -S --noconfirm base-devel git sudo \
    && useradd -m -s /bin/bash dev \
    && echo "dev ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/dev

# Set the default shell to bash
SHELL ["/bin/bash", "-c"]

USER dev
WORKDIR /home/dev
