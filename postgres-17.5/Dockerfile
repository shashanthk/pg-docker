# Dockerfile
FROM postgres:17.5

# ---- Debian/Ubuntu-based tags (the default “postgres:x.y”) ----
RUN set -eux; \
    apt update; \
    apt install -y --no-install-recommends postgresql-plperl-17; \
    rm -rf /var/lib/apt/lists/*

RUN mkdir -p /data/tmp && chmod 1777 /data/tmp