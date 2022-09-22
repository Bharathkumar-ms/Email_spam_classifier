# Email Spam-Classifier

## Heroku link

**click this**<br>
[EMail Spam Classifier](https://email-spam-classifier-5.herokuapp.com/)



### Docker Image

    FROM python:3.10
    COPY . /app
    WORKDIR /app
    RUN pip install -r requirements.txt
    EXPOSE $PORT
    CMD gunicore --workers=4 --bind 0.0.0.0:$PORT aap:app
    
    
### Procfile
    web gunicorn app:app

### Screenshot

![Screenshot (389)](https://user-images.githubusercontent.com/96257624/191796006-c6fd050c-197f-4860-9c8d-382ffe70ccfe.png)
