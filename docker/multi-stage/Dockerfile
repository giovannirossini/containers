FROM ubuntu:20.04 AS deno

RUN apt-get update && apt-get install -yf curl unzip
RUN curl -fsSL https://deno.land/x/install/install.sh | sh

FROM ubuntu:20.04

COPY --from=deno /root/.deno/bin/deno /usr/local/bin/deno

ADD ./ /app

WORKDIR /app

EXPOSE 3000
