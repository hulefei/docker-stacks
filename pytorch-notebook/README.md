# Jupyter Notebook Deep Learning Stack

[![docker pulls](https://img.shields.io/docker/pulls/jupyter/tensorflow-notebook.svg)](https://hub.docker.com/r/jupyter/tensorflow-notebook/)
[![docker stars](https://img.shields.io/docker/stars/jupyter/tensorflow-notebook.svg)](https://hub.docker.com/r/jupyter/tensorflow-notebook/)
[![image size](https://img.shields.io/docker/image-size/jupyter/tensorflow-notebook/latest)](https://hub.docker.com/r/jupyter/tensorflow-notebook/ "jupyter/tensorflow-notebook image size")

GitHub Actions in the <https://github.com/jupyter/docker-stacks> project builds and pushes this image to Docker Hub.

Please visit the project documentation site for help to use and contribute to this image and others.

- [Jupyter Docker Stacks on ReadTheDocs](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
- [Selecting an Image :: Core Stacks :: jupyter/tensorflow-notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-tensorflow-notebook)
- [Image Specifics :: Tensorflow](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/specifics.html#tensorflow)


# Run
docker build -t hulefei/jupyter:pytorch .

# Build
docker run --gpus all --rm -d -p 8888:8888 -v /cfs/jovyan/work:/home/jovyan/work hulefei/jupyter:pytorch start-notebook.sh --NotebookApp.token='a1'