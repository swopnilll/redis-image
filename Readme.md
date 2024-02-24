# Creating Custom Docker Images with Dockerfile

## Introduction

 In this, we'll create a Dockerfile to build an image that runs a Redis server.

## Project Setup

1. **Create Working Directory**: Begin by creating a new directory named `Redis Image`.
2. **Open Code Editor**: Navigate to the newly created directory and open it in your preferred code editor.

## Creating Dockerfile

1. **Create Dockerfile**: Inside the `Redis Image` directory, create a new file named `Dockerfile` (note the capital 'D' and no file extension).

2. **Define Comments**: Write comments inside the Dockerfile to guide through the image creation process. Comments include:

   - Using an existing Docker image as a base.
   - Downloading and installing dependencies.
   - Specifying container startup commands.

3. **Write Dockerfile Configuration**:

   ```dockerfile
   # Use Alpine as base image
   FROM Alpine

   # Download and install Redis dependency
   RUN apk add --update Redis

   # Specify command to run Redis server when container starts
   CMD ["Redis-server"]
   ```
