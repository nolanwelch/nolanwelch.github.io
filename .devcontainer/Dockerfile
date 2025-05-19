FROM node:23-slim

ENV NODE_ENV=development

WORKDIR /workspace

# Install essential packages
RUN apt-get update && apt-get install -y \
    curl \
    git \
    gcc \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

# Install Hugo
RUN apt-get install hugo

# Hugo
EXPOSE 1313

# node user
USER 1000