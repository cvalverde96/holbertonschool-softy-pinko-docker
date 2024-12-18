# Is based on the latest ubuntu
FROM ubuntu:latest

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software through APT using apt-get upgrade -y
RUN apt-get upgrade -y

# Install python3, python3-pip, flask, and flask_cors
RUN apt-get install -y python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask
RUN pip3 install flask_cors

# use /app as the working directory and copy the Python file to your Docker image
WORKDIR /app
COPY api.py /app/api.py

# Expose port 5252 for the Flask application
EXPOSE 5252

# Once built, you can run the Docker image in a container and it will echo “Hello, World!” on the terminal.
CMD ["python3", "api.py"]

# commands to run for verification
# docker build -f ./front-end/Dockerfile -t softy-pinko-front-end:task2 ./front-end /It creates a Docker image named softy-pinko with the version task1.
# docker run -p 9000:9000 -it --rm --name softy-pinko-front-end-task2 softy-pinko-front-end:task2 /It starts a temporary container interactively, and the container is deleted after it stops.
