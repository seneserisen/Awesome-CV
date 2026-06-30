FROM texlive/texlive:latest

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y --no-install-recommends fonts-roboto fonts-adobe-sourcesans3 && rm -rf /var/lib/apt/lists/*

WORKDIR /doc
CMD ["make"]
