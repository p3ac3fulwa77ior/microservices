FROM craicerjack/nginx-flask
WORKDIR /usr/src/app

COPY . .

EXPOSE 6003

CMD ["python","setup.py"]
CMD ["python","bookings.py &"]

