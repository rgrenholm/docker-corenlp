    docker system prune -a
    docker build -t corenlp .
    docker run -d -p 9000:9000 corenlp
