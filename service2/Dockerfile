FROM craicerjack/nginx-flask
WORKDIR /usr/src/app

COPY . .

EXPOSE 6003

RUN make install
RUN make launch
