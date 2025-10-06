# MULTI-CONTAINER-APPLICATION-USING-DOCKER-FOR-AUTOMATION


In this project, I have set up three containers: a client, a server, and a worker. 
#client
The client container is responsible for serving the front-end React application, 

#server
while the server container is responsible for handling the business logic and communicating with the RDS database to fetch the Fibonacci numbers. 

#worker
The worker container is responsible for performing the actual calculation of Fibonacci numbers and storing the results in the RDS database.

#connecting containers
To connect the containers, I have used Docker Compose, which is a tool for defining and running multi-container Docker applications. 
Docker Compose allows you to specify the configuration for each container, as well as define the network and volume settings for the application.

#deployment
As part of the CI/CD pipeline, i have set up a Travis-CI job to automatically build and test the Docker images for the client, server, and worker containers.
Once the images have been successfully built and tested, they are pushed to the Docker registry on AWS.
For deployment, I have configured AWS Elastic Beanstalk to automatically deploy the Docker images to the appropriate EC2 instances.

#use case
Elastic Beanstalk automatically creates the necessary infrastructure to run the containers, including load balancers and auto-scaling groups.
To store the Fibonacci numbers in the RDS database, you have set up a PostgreSQL database on AWS. 
The server container communicates with the RDS database using a connection string that specifies the host, port, database name, username, and password.
Overall, your project is a great example of how Docker and CI/CD pipelines can be used to build, test, and deploy multi-container applications.
By using tools like Docker Compose, Travis-CI, and AWS, I have made it easy to manage the infrastructure for the application, 
while ensuring that it is reliable, scalable, and secure.

###SKILLS
Docker, React.js, Git, Github, Travis-ci, AWS, CI/CD

