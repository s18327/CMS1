# CMS1

## Try it

```bash
git clone https://github.com/s18327/CMS1.git
cd CMS1
docker compose build web
docker compose up -d database_default
docker compose run web python manage.py migrate
docker compose run web python manage.py createsuperuser
docker compose up -d
```

Then open http://django-cms-quickstart.127.0.0.1.nip.io:8000 (or just http://127.0.0.1:8000) in your browser.
