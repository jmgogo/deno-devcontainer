# Comments are provided throughout this file to help you get started.
# If you need more help, visit the Dockerfile reference guide at
# https://docs.docker.com/engine/reference/builder/

# Latest version of Deno on Debian
FROM denoland/deno:debian as devcontainer

# Update the system and install necessary packages
RUN apt update  \
    && apt upgrade -y  \
    # Install Jupyter
    && apt install -y jupyter \
    # Install Deno kernel for jupyter
    && deno jupyter --install \
    # Clean up the system to reduce image size
    && apt clean \
    && rm -rf /var/lib/apt/lists/* 

# set working directory
WORKDIR /home/deno

CMD ["sleep", "infinity"]