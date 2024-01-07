```
docker build -t aspnetcore-hello -f Dockerfile .
docker run -p 8085:8080 aspnetcore-hello

curl http://localhost:8085
ab -c 50 -n 5000 http://localhost:8085/
k6 run ./api-test.js
```