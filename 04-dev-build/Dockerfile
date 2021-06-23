# docker image build -t dev-build .
# docker container run -it -v $(pwd):/app -p 8080:8000 --name python-server dev-build

FROM python:3.6
RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log
USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD ["run.py"]