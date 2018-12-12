FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN node -v && npm -v

COPY ./frontend-example-docker .
RUN npm install

EXPOSE 5000
ENV API_URL=http://localhost:8000
CMD npm start

# docker build -t fed
# docker run --rm -p 5001:5000 fed
