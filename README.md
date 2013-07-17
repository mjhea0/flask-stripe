flask-stripe
========================

Use this app to integrate Flask and Stripe with a simple user registration system. After user registration, the user is taken to a memeber's page where s/he can then purchase premium content via Stripe.

- Flask==0.10.1
- Flask-SQLAlchemy==0.16
- Flask-WTF==0.8.4
- Jinja2==2.7
- MarkupSafe==0.18
- SQLAlchemy==0.8.2
- WTForms==1.0.4
- Werkzeug==0.9.1
- itsdangerous==0.22
- requests==1.2.3
- stripe==1.9.2
- wsgiref==0.1.2
 
## Setup

1. clone the repo
2. setup/activate a virtualenv
3. install the requirements
4. update the rdms (sqlite, mysql, postgres)
5. create the database (*db_create.py*)
6. Update the amount charged in the controller, *views.py*, and the subsequent views, *memebers.html* and *charge.html*.

## Todo

1. create better documentation
2. add unit tests
3. add email verification
4. add the ability to make a subscription purchase as well
5. create a payment form instead of the generic stripe popup

## Screenshot

![djang-stripe](http://content.screencast.com/users/Mike_Extentech/folders/Jing/media/754f9275-d5e4-4aa9-bfcf-a0f6fbebf63b/00000211.png)

## Project structure

    ├── app
    │   ├── __init__.py
    │   ├── forms.py
    │   ├── keys.cfg
    │   ├── models.py
    │   ├── templates
    │   │   ├── 404.html
    │   │   ├── 500.html
    │   │   ├── base.html
    │   │   ├── charge.html
    │   │   ├── login.html
    │   │   ├── members.html
    │   │   └── register.html
    │   └── views.py
    ├── config.py
    ├── db_create.py
    ├── error.log
    ├── requirements.txt
    └── run.py
