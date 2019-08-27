    docker system prune -a
    docker build -t corenlp-tag https://github.com/rgrenholm/docker-corenlp.git
    docker run -d -p 9000:9000
    
    docker network create -d bridge corenlp-net
    docker run -d -p 9000:80 --network="corenlp-net" --name corenlp-inst
