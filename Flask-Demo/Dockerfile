
FROM kennethreitz/pipenv

WORKDIR /app

COPY . /app/

RUN pipenv install --deploy --system

EXPOSE 8000

CMD ["gunicorn", "main:app", "-b", "0.0.0.0:8000"]
