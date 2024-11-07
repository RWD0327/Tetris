# Dockerfile
FROM archlinux:latest

# 기본 패키지 업데이트 및 설치
RUN pacman -Syu --noconfirm \
    && pacman -S --noconfirm base-devel git sudo \
    && useradd -m -s /bin/bash dev \
    && echo "dev ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/dev

USER dev
WORKDIR /home/dev
