FROM ubuntu

# install deps
RUN apt-get update && apt-get install -y curl

RUN mkdir /build /cache /env
WORKDIR /buildpack
COPY bin/compile bin/detect bin/release /buildpack/bin/
RUN /buildpack/bin/compile /build /cache /env

# test with sample.tex
COPY test/sample.tex /build/sample.tex
RUN /build/pandoc-bin/usr/bin/pandoc /build/sample.tex