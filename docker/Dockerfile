FROM python:3.10.0b4

RUN pip install --upgrade pip pipenv

WORKDIR /src/stringsifter
COPY . /src/stringsifter

RUN pipenv install --system --deploy
RUN pip install -e /src/stringsifter

CMD [ "/bin/bash" ]
