## aws-glue-etl-local-docker
[Link to Docker Image](https://hub.docker.com/repository/docker/jnshubham/glue_etl_local)

This docker image is used to run your glue etl jobs on your local environment.
This helps in the development of etl jobs locally without incurring additional costs by running Glue Devendpoints or Glue jobs.

Having glue libraries locally helps in the development and making it easier for the developer to update/change the code and test it locally before commiting it to a job.

### Build Image Manually
To build the image on your system, follow these steps:
1. Clone the repository to get the latest Dockerfile

```
git clone https://github.com/jnshubham/aws-glue-local-etl-docker.git
```

2. Start Docker

```
system start docker
```

3. Run build command

```
docker build -t jnshubham/glue_etl_local .
```

4. Once the build is successful, run the container using commands in Run section.



### To get the prebuild image directly
Run

```
docker pull jnshubham/glue_etl_local:latest
```

Check downloaded image by running
```
docker images
```

### Commands to run the container
To run the container and get into pyspark shell directly

```
docker run jnshubham/glue_etl_local "gluepyspark"
```

To get into the terminal and submit a job run

```
docker run -it jnshubham/glue_etl_local

gluesparksubmit script_name parameters
```

To checkout the image visit [Docker page here](https://hub.docker.com/repository/docker/jnshubham/glue_etl_local)

Thanks!
