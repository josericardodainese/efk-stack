# fluentd/Dockerfile

FROM fluent/fluentd:v1.14.5-debian-1.0
USER root
RUN ["gem", "uninstall", "-I", "elasticsearch"]
RUN ["gem", "install", "elasticsearch", "-v", "7.13.3"]
RUN ["gem", "install", "fluent-plugin-multi-format-parser", "-v", "1.0.0"]
RUN ["gem", "install", "fluent-plugin-elasticsearch", "--no-document", "--version", "5.0.3"]
USER root