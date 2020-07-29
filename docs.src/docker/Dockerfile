FROM python:3.7

RUN \
	pip install --upgrade pip && \
	pip install pathlib mkdocs mkdocs-material mkdocs-markdownextradata-plugin

WORKDIR /development
ENTRYPOINT [ "mkdocs", "serve", "--dev-addr", "0.0.0.0:8000", "--config-file" ]
CMD [ "mkdocs.yml" ]
