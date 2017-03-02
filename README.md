# Legalstart Test Instructions

You will receive further instructions right before the interview.

## How to run?

Choose the way you are more conforable with. Either:
- venv
- Docker
- docker-compose

### venv

```
cd core
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py runserver 0.0.0.0:5678
```

### Docker

```
docker build core/ --tag wip
docker run --publish 5678:5678 wip
```

### docker-compose

```
docker-compose up --build
```

## Suggestions

- There is no wrong answer; only wrongly justified answers.
- Any commit is better than no commit; few small commits are better than one large commit.