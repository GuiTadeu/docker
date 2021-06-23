# docker image build --build-arg S3_BUCKET=myapp -t arg-build .
# docker container run arg-build bash -c 'echo $S3_BUCKET'
# return: myapp

FROM debian
ARG S3_BUCKET=files
ENV S3_BUCKET=${S3_BUCKET}