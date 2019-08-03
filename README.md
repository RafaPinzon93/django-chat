# Rapid-ChatXChannels
An implementation of the tutorial and introduction of Django Channels. To get more in-depth check out the full course https://kirr.co/badl8e

Additionally, I used Docker to run Django, Redis and Postgres.

## Instructions

__Prerequisites__: Docker, docker-compose

1. Clone or download the project
```bash
git clone https://github.com/RafaPinzon93/django-chat.git
```
2. Run ```docker-compose build```
3. Execute the migrations ```docker-compose run web python manage.py migrate```
4. Create __TWO__ superusers. ```docker-compose run web python manage.py createsuperuser```
5. Run the application. ```docker-compose run```
6. Go to http://localhost:8000/admin, login with one user.
7. Open an incognito or another browser and login with the other user.
8. Go to http://localhost:8000/messages/[other_user_name] where "other_user_name" is the name of the user we are going to talk (different to himself).
