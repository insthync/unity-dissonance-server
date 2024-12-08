FROM ubuntu:18.04
LABEL maintainer="ittipon.bay@gmail.com"

# Set the working directory
WORKDIR /unity-server

# Copy the Unity build to the container
COPY . /unity-server

# Ensure the server binary has execution permissions
RUN chmod +x /unity-server/App.x86_64

# Expose any ports the server needs to communicate on
EXPOSE 3000/tcp 3000/udp

# Define the command to run the server
CMD ["./App.x86_64", "-batchmode", "-nographics", "-logfile", "/dev/stdout"]