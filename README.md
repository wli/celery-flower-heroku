Deploy [Flower](https://github.com/mher/flower/) to Heroku to monitor [Celery](http://www.celeryproject.org/).

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Configure the app by providing your broker url (RabbitMQ, Redis, what have you) and the Google OpenID auth email domain for logging into Flower:

```bash
heroku config:set BROKER_URL=redis://...
heroku config:set FLOWER_EMAIL_DOMAIN=".*@example\.com$"
```
