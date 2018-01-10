# celery-flower-redis
deploy Celery with Redis and Flower using Docker

what you need to do:
change the 'volumes' path in 'docker-compose.yml'
```
# celery-worker.py
# !usr/bin/python

from celery import Celery
app = Celery("cef")


@app.task
def add(x, y):
    return x + y

```

