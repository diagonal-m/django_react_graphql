# django_react_graphql

## Docker 操作方法

```bash
$ pwd
/django_react_graphql
$ ls
README.md  django_graphql/ docker/
$ docker build -f docker/Dockerfile -t django --no-cache .
$ docker run --name django -it --rm -v $(pwd):/tmp -p 8000:8000 django:latest /bin/bash
$ cd django_graphql
$ python manage.py runserver 0.0.0.0:8000
```
