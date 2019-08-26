docker system prune -a <br>
docker build -t corenlp . <br>
docker run -d -p 9000:9000 corenlp <br>
