# Two-Tier Flask App with MySQL (Dockerized)
This project demonstrates running a Flask web app and a MySQL database in separate Docker containers that communicate through a custom Docker network.

## Steps to run the project:
Clone the GitHub repository and navigate into the project directory.

Create and Build the Docker image for the Flask app using the provided Dockerfile.

Create a custom Docker network (e.g., two-tier) to allow communication between containers.

Run the MySQL container using Docker, attach it to the created network, and pass the necessary environment variables (root password and database name).

Run the Flask app container, attach it to the same network, and pass environment variables including the MySQL host (use the MySQL container name), user, password, and database name.

Open a browser and go to http://:5000 to access the Flask app. Make sure port 5000 is allowed through any firewall or VM network rules.
