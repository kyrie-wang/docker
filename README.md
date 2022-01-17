# docker

## Command
1. How to rename images \"REPOSITORY\" and \"TAG\"
    ```
    docker tag IMAGEID REPOSITORY:TAG
    ```
2. How to create image from container
    ```
    docker commit -a "AUTHER" -m "MESSAGE" CONTAINER REPOSITORY:TAG
    ```
3. How to save image to ```*.tar.gz```
    ```
    docker save -o *.tar.gz IMAGE [IMAGE...]
    ```
4. How to load iamge from ```*.tar.gz```
    ```
    docker load -i *.tar.gz
    ```

## Install Dockfile
```
docker build -t ${NAME}:${TAG} -f ubuntu\:20.04/base/Dockerfile.base .
```