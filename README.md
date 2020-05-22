# tweet-spark

## WorkFlow


![](src/docker_pyspark.png)


- Downloading and running the container
  
  To create and start a container with Spark, PySpark, SciPy, and Jupyter, run the following command in your terminal.

```
$ docker run --name sparkbook -p 8881:8888 -v "$PWD":/home/jovyan/work jupyter/pyspark-notebook start.sh jupyter lab --LabApp.token=''
```

- To start this container up in the future, you only need to type

```
$ docker start sparkbook  
```

- Accessing the Jupyter server running in the container

 open to web browser, type ```localhost:8882```
 
![Geopandas](src/gp.png) 

- install geopandas packages on the container

```$ docker exec -it sparkbook bash
jovyan@839db31a6a90:~$ pip install geopandas
jovyan@839db31a6a90:~$ pip install descartes
```


## About Data
 - 216,912 rows corresponding to individual tweets. Over 60 features.
 - Tweets are in French with accounts predominately located in France at the time of the tweet.
 - Information gathered during April 26 -29 2017
