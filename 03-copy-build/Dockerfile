# docker image build -t copy-build .
# docker container run -p 8080:80 copy-build

FROM nginx:latest
RUN echo '<h1>Sem Conteúdo</h1>' > /usr/share/nginx/html/conteudo.html
COPY *.html /usr/share/nginx/html/