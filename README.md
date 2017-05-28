# Project create
Ageeva Tatiana
4-47

Для начала можно использовать - вот такой контейнер https://hub.docker.com/r/jupyter/scipy-notebook/
Однако его Docker файл позднее придется пересобрать. Проблема - в иерархии зависимостей и большом размере контейнера - 4.5 Gb - за гранью добра и зла.
Docker файл взят вот отсюда
https://github.com/jupyter/docker-stacks/tree/master/scipy-notebook
Для работы с OpenCV можно взять файл opencv/TestVideo, предварительно загрузив его в JupyterNotebook. Команда для JupyterNotebook with OpenCV: docker run --rm -it --name alpine-jupyter-01 --device /dev/video0:/dev/video0 -p 8888:8888 eipdev/alpine-jupyter-notebook


