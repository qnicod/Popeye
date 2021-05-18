# Popeye

During this project, you are going to master the basics of containerizing applications and describing multi-containers infrastructures with Docker and Docker Compose.

You will have to containerize and define the deployment of a simple web poll application.There are five elements constituting the application:-Poll, a Flask Python web application that gathers votes and push them into a Redis queue.- ARedis queue, which holds the votes sent by the Poll application, awaiting for them to be consumed bythe Worker.

- The Worker, a Java application which consumes the votes being in the Redis queue, and stores them intoa PostgreSQL database.
- A PostgreSQL database, which (persistently) stores the votes stored by the Worker.
- Result,a Node.js web application that fetches the votes from the database and displays the... well,result.
