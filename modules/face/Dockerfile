FROM ubuntu:latest

LABEL authors="daiego"
LABEL description="Image to run HeWo with proper dependencies and persistent venv"

# ── Base dependencies ─────────────────────────────
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    python3-venv \
    libgl1 \
    libglib2.0-0 \
    x11-utils \
    x11-xserver-utils \
    libxrandr-dev \
    ffmpeg

# ── Copy source ───────────────────────────────────
RUN python3 -m pip install --break-system-packages hewo-face