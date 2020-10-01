# spring-boot-microservice-with-eureka
<br>this project uses Ribbon to make the load balance,
<br>eureka config server to keep the configs,
<br>and the eureka server to get the id of each application,
<br>https://spring.io/projects/spring-cloud-netflix
<br>
<b>to run this project:</b>
<br>mysql:
<br>docker run --name mysql-fornecedor -e MYSQL_USER=root -e MYSQL_DATABASE=fornecedor -e   MYSQL_ROOT_PASSWORD=root -d -p 3306:3306 mysql:5.6
<br>
cd /config-server/ 
<br>./mvnw spring-boot:run

<br>cd /eureka-server/ 
<br>./mvnw spring-boot:run

<br>cd /fornecedor/ 
<br>./mvnw spring-boot:run

<br>cd /loja/ 
<br>./mvnw spring-boot:run
