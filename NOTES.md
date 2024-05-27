# Start rudolfs
```sh
git clone https://github.com/jasonwhite/rudolfs/
docker run -it jasonwhite0/rudolfs:latest local
openssl rand -hex 32 > key.txt
KEY=$(cat key.txt) docker run -it -p 8080:8080  jasonwhite0/rudolfs:latest --key=$KEY --port 8080 local --path=./data
```
