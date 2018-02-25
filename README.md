# Python notebooks
This repository is for backing up my python notebooks.

## Notebook
I use [Jupyter notebook](http://jupyter.org/) both for R and Python codes. [IRkerlen](https://github.com/IRkernel/IRkernel) should be installed for running R codes via Jupyter. 

I used a docker image for running these notebooks. 

### List of notebook images
* Python: [avikdatta/pythonjupyterdockerimage](https://hub.docker.com/r/avikdatta/pythonjupyterdockerimage/) 

    [![DockerPulls](https://img.shields.io/docker/pulls/avikdatta/pythonjupyterdockerimage.svg)](https://registry.hub.docker.com/u/avikdatta/pythonjupyterdockerimage/) [![](https://images.microbadger.com/badges/image/avikdatta/pythonjupyterdockerimage.svg)](https://microbadger.com/images/avikdatta/pythonjupyterdockerimage)

* R: [avikdatta/rjupyterdockerimage](https://hub.docker.com/r/avikdatta/rjupyterdockerimage/) 

    [![DockerPulls](https://img.shields.io/docker/pulls/avikdatta/rjupyterdockerimage.svg)](https://registry.hub.docker.com/u/avikdatta/rjupyterdockerimage/) [![](https://images.microbadger.com/badges/image/avikdatta/rjupyterdockerimage.svg)](https://microbadger.com/images/avikdatta/rjupyterdockerimage)

* Apache Spark (pyspark): [avikdatta/sparkjupyterdockerimage](https://hub.docker.com/r/avikdatta/sparkjupyterdockerimage/)

    [![DockerPulls](https://img.shields.io/docker/pulls/avikdatta/sparkjupyterdockerimage.svg)](https://registry.hub.docker.com/u/avikdatta/sparkjupyterdockerimage/) [![](https://images.microbadger.com/badges/image/avikdatta/sparkjupyterdockerimage.svg)](https://microbadger.com/images/avikdatta/sparkjupyterdockerimage)

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
## List of notebooks

#### Spark notebooks
* [Speark streaming using a socket source](spark/spark_streaming/spark_streaming_socket.ipynb)
* [Speark stream using a kafka data source](spark/spark_streaming/spark_streaming_kafka.ipynb)

#### Slack bots
* [A basic slack bot](bot/slack/slack_bot_test1_20170714.ipynb)
* [A basic IGF data fetching bot](bot/slack/slack_bot_test2_20180206.ipynb)

#### Twitter bot
* [A basic twitter dm bot for IGF](bot/twitter_bot/basic_igf_tweet_dm_bot.ipynb)

