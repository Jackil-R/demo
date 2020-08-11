# demo
spring boot demo

Make sure you have docker install.

Start the postgres database by running following in the terminal:

docker run --name postgres-spring -e POSTGRES_PASSWORD=password -d -p 5432:5432 postgres:alpine

Onc the db is up, start the application.

Go to the demo directory and run the cmd below.

mvn clean package 

Then change directory to the target directory and run the cmd below.

java -jar demo-0.0.1-SNAPSHOT.jar

Use generated-requests.http in Intellij to make request to the backend service.