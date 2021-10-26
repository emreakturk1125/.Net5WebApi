# .Net5WebApi
 .Net 5 Web API, Mongo Db, Docker, Kubernetes, UnitTest
 
# Source code

If You download source code;
<br>
After "docker run" on terminal 

Primary Key is Guid Id 
<br>
GetById -> https://localhost:5001/items/1f5b9837-010c-4042-9f29-25a919807053
<br>
GetAll ->    https://localhost:5001/items
<br>
Post ->        https://localhost:5001/items
<br>
Delete ->   https://localhost:5001/items/a350187a-cd67-4e9d-8786-eeabbf6b1fce 

# Docker Hub 

docker pull emreakturk/catalogapiexample
<br>
docker run -p 5000:80 -d emreakturk/catalogapiexample  
<br>
docker run -d --rm --name mongo -p 27017:27017 -v mongodbdata:/data/db -e MONGO_INITDB_ROOT_USERNAME=mongoadmin -e MONGO_INITDB_ROOT_PASSWORD=Pass#word1 --network=catalogexample emreakturk/catalogapiexample mongo
<br>
<br>
docker run -it --rm -p 8080:80 -e MongoDbSettings:Host=mongo -e MongoDbSettings:Password:Pass#word1 --network=catalogexample emreakturk/catalogapiexample
<br>
Primary Key is Guid Id 
<br>
GetById -> https://localhost:8080/items/1f5b9837-010c-4042-9f29-25a919807053
<br>
GetAll ->    https://localhost:8080/items
<br>
Post ->        https://localhost:8080/items
<br>
Delete ->   https://localhost:8080/items/a350187a-cd67-4e9d-8786-eeabbf6b1fce 
