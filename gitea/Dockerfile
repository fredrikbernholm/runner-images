FROM gitea/runner-images:ubuntu-latest

USER root

RUN npx -y playwright-core@1.64.1 install-deps chromium firefox

RUN apt-get update && apt-get install -y --no-install-recommends \
  curl git-lfs ca-certificates \
  && rm -rf /var/lib/apt/lists/*
