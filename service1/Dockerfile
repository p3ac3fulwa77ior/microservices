FROM craicerjack/nginx-flask
WORKDIR /usr/src/app

COPY . .

EXPOSE 6001

CMD ["python","setup.py"]
CMD ["python","movies.py &"]

