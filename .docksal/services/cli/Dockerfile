# Use a stock Docksal image as the base
FROM docksal/cli:2.1-php7.1

ARG HUGO_VERSION

# Install hugo.
RUN wget -q https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_${HUGO_VERSION}_Linux-64bit.deb -O /tmp/hugo.deb \
        && dpkg -i /tmp/hugo.deb \
        && apt-get update; apt-get -y install python-docutils
