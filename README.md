# Aubay-Orc
Oracle Challenge

## Expected behaviour

- Developers can trigger the pipeline with parameters (Environment name, MySQL password and MySQL port)
- A docker image built from latest MySQL image
- Spin up a container from the image built above, exposing the requested port on the Docker host
- Prepare the environment by creating an account for the developer (username: developer, password: based on input parameter)
