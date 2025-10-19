FROM alpine

RUN apk add curl

COPY smoke-test.sh smoke-test.sh

CMD ["sh", "smoke-test.sh", "http://app:3000"]

#packages install
RUN npm i

# tests
RUN npm run test
