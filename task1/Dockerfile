# Is based on the latest ubuntu
FROM ubuntu:latest

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software through APT using apt-get upgrade -y
RUN apt-get upgrade -y

# Install python3, python3-pip, and flask
RUN apt-get install -y python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask

# use /app as the working directory and copy the Python file to your Docker image
WORKDIR /app
COPY api.py /app/api.py

# Expose port 5252 for the Flask application
EXPOSE 5252

# Once built, you can run the Docker image in a container and it will echo “Hello, World!” on the terminal.
CMD ["python3", "api.py"]

# commands to run for verification
# docker build -f ./Dockerfile -t softy-pinko:task1 . /It creates a Docker image named softy-pinko with the version task1.
# docker run -p 5252:5252 -it --rm --name softy-pinko-task1 softy-pinko:task1 /It starts a temporary container interactively, and the container is deleted after it stops.
# Remember to go to this endpoint: http://localhost:5252/api/hello
