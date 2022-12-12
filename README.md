# Docker Devops

## CLI commands

**Building docker image**

``
docker build -t devops-kpi .
``

**Run docker container with limits for cpu and memory and available on port 80

```
docker run -d --rm --memory=50m --cpus="1.0" --name kpi -p 80:80 devops-kpi
```

**Push docker image to docker hub**

```
docker build -t VladPetrushchenko/devops-kpi
```

After that we're ready to push it to our repo

```
docker login

docker push VladPetrushchenko/devops-kpi
```
