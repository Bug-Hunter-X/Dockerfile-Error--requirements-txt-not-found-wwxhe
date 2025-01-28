# Dockerfile Bug: Missing requirements.txt

This repository demonstrates a common error in Dockerfiles where the application fails because it can't locate the `requirements.txt` file during the build process.

The `Dockerfile` attempts to install dependencies using `pip3 install -r requirements.txt`. However, the location where `requirements.txt` is copied into the image is incorrect causing the `pip3` command to fail.