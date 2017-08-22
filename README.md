# QUICKSTART

```
git clone <url> mydir && cd mydir
docker run --rm -it \
    -v `pwd`:/pwd \
    -w /pwd \
    -p 8080:8080 \
    python:3.6-alpine \
    sh -c 'pip install -r requirements.txt \
        && cd mysite \
        && python manage.py runserver 0:8080'
```

