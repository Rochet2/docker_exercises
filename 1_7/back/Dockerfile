FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN node -v && npm -v

COPY ./backend-example-docker .
RUN npm install

EXPOSE 8000
CMD FRONT_URL=http://localhost:5001 npm start

# docker build -t bed .
# docker run --rm -p 8000:8000 -v $(pwd)/backend-example-docker/logs.txt:/mydir/logs.txt bed
