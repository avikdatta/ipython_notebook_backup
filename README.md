# ipython_notebook_backup
A repository for ipython notebook backup

I use [Jupyter notebook](http://jupyter.org/) both for R and Python codes. [IRkerlen](https://github.com/IRkernel/IRkernel) should be installed for running R codes via Jupyter. 

I used a docker image for running this data analysis script. This image could be built either using the docker file from this git repo, [python_docker_file](https://github.com/avikdatta/python_data_docker_files/tree/master/python_docker_file) or it can be fetched directly from the docker hub [python docker image](https://hub.docker.com/r/avikdatta/python_data/)

## Docker run command
<pre><code>
  docker run -it -v /path:/root/app -p 8888:8888 avikdatta/py_hadoop_data:latest jupyter-notebook --ip 0.0.0.0  
</code></pre>
