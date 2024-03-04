FROM python:3.11-rc-slim@sha256:a7b7703e1479bce7e911341cac76c3cad4d1b7efa794f03fc2df17155152fef0

RUN pip install --upgrade pip pipenv

WORKDIR /src/stringsifter
COPY . /src/stringsifter

RUN pipenv install --system --deploy
RUN pip install -e /src/stringsifter

CMD [ "/bin/bash" ]
