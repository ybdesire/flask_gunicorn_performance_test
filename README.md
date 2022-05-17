# flask_gunicorn_performance_test
performance test with or without gunicorn

# environment
* ubuntu
* python 3.8.10

# 1. run server

1. `python server.py`
2. `curl http://localhost:8002/todos?task=jobs&my_list=[1,2,3]`
3. by code reference: https://github.com/ybdesire/pylearn/blob/master/flask_restful/post_list/http_post.ipynb


# 2. install ab

```
ubuntu@VM-4-15-ubuntu:~$ sudo apt-get install apache2-utils

```


# 3. performance test by ab command


1. basic

```
ubuntu@VM-4-15-ubuntu:~$ ab -n 10000 -c 500 http://localhost:8002/todos?task=jobs&my_list=[1,2,3]
```

* total 10000 requests
* concurrency is 500

2. output


3. references

https://fang.readthedocs.io/zh_CN/latest/%E8%BF%90%E7%BB%B4%E4%BA%BA%E7%94%9F/%E7%BD%91%E7%AB%99%E6%80%A7%E8%83%BD%E5%8E%8B%E5%8A%9B%E6%B5%8B%E8%AF%95%E4%B9%8Bab%E5%91%BD%E4%BB%A4.html

# 4. performance test by jmeter




