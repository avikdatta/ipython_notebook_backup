# Python notebooks
This repository is for backing up my python notebooks.

## Notebook
I use [Jupyter notebook](http://jupyter.org/) both for R and Python codes. [IRkerlen](https://github.com/IRkernel/IRkernel) should be installed for running R codes via Jupyter. 

I used a docker image for running this data analysis script. This image can be built either using the docker file from this git repo, [python_docker_file](https://github.com/avikdatta/python_data_docker_files/tree/master/python_docker_file), or it can be fetched directly from the docker hub [python docker image](https://hub.docker.com/r/avikdatta/python_data/)

### List of notebook images
* Python: [avikdatta/pythonjupyterdockerimage](https://hub.docker.com/r/avikdatta/pythonjupyterdockerimage/) [![DockerPulls](https://img.shields.io/docker/pulls/avikdatta/pythonjupyterdockerimage.svg)](https://registry.hub.docker.com/u/avikdatta/pythonjupyterdockerimage/) [![](https://images.microbadger.com/badges/image/avikdatta/pythonjupyterdockerimage.svg)](https://microbadger.com/images/avikdatta/pythonjupyterdockerimage)

* R: [avikdatta/rjupyterdockerimage](https://hub.docker.com/r/avikdatta/rjupyterdockerimage/) [![DockerPulls](https://img.shields.io/docker/pulls/avikdatta/rjupyterdockerimage.svg)](https://registry.hub.docker.com/u/avikdatta/rjupyterdockerimage/) [![](https://images.microbadger.com/badges/image/avikdatta/rjupyterdockerimage.svg)](https://microbadger.com/images/avikdatta/rjupyterdockerimage)
* Apache Spark (pyspark): [avikdatta/sparkjupyterdockerimage](https://hub.docker.com/r/avikdatta/sparkjupyterdockerimage/) 
[![](https://images.microbadger.com/badges/image/avikdatta/sparkjupyterdockerimage.svg)](https://microbadger.com/images/avikdatta/sparkjupyterdockerimage)

## Docker run command
```bash
  docker run 
    -it \
    -v /path:/root/app \
    -p 8888:8888 \
    avikdatta/pythonjupyterdockerimage \
    jupyter-notebook \
    --ip 0.0.0.0  
```
