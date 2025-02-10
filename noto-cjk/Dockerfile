ARG VERSION=
FROM chromedp/headless-shell:${VERSION}

RUN \
  apt-get update -y \
  && apt-get install -y \
  locales \
  task-japanese \
  locales-all \
  fonts-noto-cjk fonts-noto-core fonts-noto-hinted \
  && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENV TZ=Asia/Tokyo
ENV LANG=ja_JP.UTF-8
