# spring-boot-microservice-with-eureka
this project uses Ribbon to make the load balance,
eureka config server to keep the configs,
and the eureka server to get the id of each application,
https://spring.io/projects/spring-cloud-netflix

to run this project:
mysql:
docker run --name mysql-fornecedor -e MYSQL_USER=root -e MYSQL_DATABASE=fornecedor -e   MYSQL_ROOT_PASSWORD=root -d -p 3306:3306 mysql:5.6

cd /config-server/ 
./mvnw spring-boot:run

cd /eureka-server/ 
./mvnw spring-boot:run

cd /fornecedor/ 
./mvnw spring-boot:run

cd /loja/ 
./mvnw spring-boot:run
