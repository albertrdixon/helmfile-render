ARG base_image=albertdixon/helmfile-render
ARG base_image_tag=latest
FROM ${base_image}:${base_image_tag}
COPY docker-entrypoint.sh /docker-entrypoint.sh
ENTRYPOINT ["/usr/bin/dumb-init", "--", "/docker-entrypoint.sh"]
