# docker-jupyter-datascience-notebook
Add library and tools to [official docker image](https://hub.docker.com/r/jupyter/datascience-notebook/)

## Added Tools
* [mecab](http://taku910.github.io/mecab/)
* [mecab-ipadic-neologd](https://github.com/neologd/mecab-ipadic-neologd)

## Usage
### Run
```console
$ docker run -it --rm -v {NOTEBOOK_MOUNT_PATH}:/work -p 8888:8888 ryutah/jupyter-datascience
```

### Use mecab-python3
```python
mecab = Mecab.Tagger("-d /usr/lib/mecab/dic/mecab-ipadic-neologd")
print(mecab.parse("こんにちは。"))
```
