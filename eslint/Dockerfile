FROM node

WORKDIR /usr/src

COPY package.json /usr/src/
RUN npm install

# COPY .eslintrc.yml /usr/src/.eslintrc.yml
COPY linter linter
RUN chmod +x linter

VOLUME /tmp

CMD ./linter
