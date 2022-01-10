FROM lscr.io/linuxserver/webtop:ubuntu-xfce

RUN set -x \
    && curl -o /tmp/gitkraken.deb https://release.axocdn.com/linux/gitkraken-amd64.deb \
    && apt-get update \
    && apt-get install -f -y ./tmp/gitkraken.deb \
    && rm -rf /var/lib/apt/lists/*

COPY root /
