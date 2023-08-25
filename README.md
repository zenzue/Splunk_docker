# Splunk_docker
Setup Splunk with docker by w01f

### Volumes

- The `volumes` section defines the "splunk_data" volume that is used by the service.

To add datasets, place the dataset files or directories in the directory associated with the "splunk_data" volume on the host machine. For example, if the Docker Compose file is located at `/path/to/docker-compose/`, place the dataset files in `/path/to/docker-compose/splunk_data/opt/splunk/var/`.

When the container is started using `docker-compose up -d`, the container will have access to the dataset files at `/opt/splunk/var/`.
