# 用Python从零开始创建区块链

## 安装

1. 安装 [Python 3.6+](https://www.python.org/downloads/) is installed. 
2. 安装 [pipenv](https://github.com/kennethreitz/pipenv). 

```
$ pip install pipenv 
```

3. 创建virtual env. 

```
$ pipenv --python=python3.6
```

4. 安装依赖.  

```
$ pipenv install 
``` 

5. 运行节点:
    * `$ pipenv run python blockchain.py` 
    * `$ pipenv run python blockchain.py -p 5001`
    * `$ pipenv run python blockchain.py --port 5002`
    
## Docker运行

另一种方式是使用Docker运行：

1. 克隆库
2. 构建docker容器

```
$ docker build -t blockchain .
```

3. 运行

```
$ docker run --rm -p 80:5000 blockchain
```

4. 添加多个节点:

```
$ docker run --rm -p 81:5000 blockchain
$ docker run --rm -p 82:5000 blockchain
$ docker run --rm -p 83:5000 blockchain
```






