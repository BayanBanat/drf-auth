
# Lab: Class 33
# drf-auth
**Author: Bayan**

**Setup**
```
python -m venv .venv      
source .venv/bin/activate 
docker-compose up          
    
```

**Testing with HTTP Clients**
manually test the API endpoints, ThunderClient

**List of Routes**

**Get Tokens**
HTTP Method: POST

**Refresh Tokens**
HTTP Method: POST


**CRUD routes for resource**

HTTP Method: GET, POST, PUT, DELETE
Token Required: Yes

**PORT** - 8000


**How to initialize/run your application**
gunicorn

Install gunicorn if you haven't already:

```
pip install gunicorn
```

**in docker-compose.yml**

```
gunicorn snacks_API.wsgi:application --bind 0.0.0.0:8000 --workers 4
```
