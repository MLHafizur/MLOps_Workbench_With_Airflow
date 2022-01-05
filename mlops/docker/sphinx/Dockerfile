ARG SPHINX_VERSION
FROM sphinxdoc/sphinx:${SPHINX_VERSION}

ENV SPHINX_OPTS=

RUN useradd -ms /bin/bash sphinxuser && \
    mkdir /mlops && \
    chown -R sphinxuser /mlops && \
    pip install sphinx_rtd_theme
USER sphinxuser

WORKDIR /mlops/docs

CMD make html SPHINXOPTS:=$SPHINX_OPTS
