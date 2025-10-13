# Use the official Node.js image
# FROM node:18.20
FROM node:22.18

# Install Git
RUN apt-get update && apt-get install -y git && apt-get clean

#copy idrsa, did not work yet for ptsisi
# COPY config/sshkey/id_ed25519 /root/.ssh/id_ed25519
# COPY config/sshkey/id_ed25519.pub /root/.ssh/id_ed25519.pub
# RUN chmod 600 /root/.ssh/id_ed25519

# Install Yarn globally
# RUN npm install -g yarn

# Set the working directory (optional)
WORKDIR /projects

# Expose a range of ports for development (optional)
EXPOSE 3021-3025

# Default command (keep the container running)
CMD ["tail", "-f", "/dev/null"]
