FROM python:3.8-slim-buster
COPY . /code
WORKDIR /code
COPY requirements.txt /code/requirements.txt
RUN python3 -m pip install --upgrade pip && \
        python3 -m pip install --trusted-host pypi.python.org -r /code/requirements.txt
EXPOSE 5001
ENTRYPOINT [ "python3" ]
CMD [ "calc.py" ]
