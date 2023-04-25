# Cinema-API

API service for manging work or the cinema.

### This project includes following features:

1. JWT authentication.
2. CRUD operations: The API includes basic CRUD (Create, Read, Update, Delete) operations
on resources such as tickets, orders, movies, cinema halls and cinema sessions.
3. Filtering movies by actors, genres and title.
4. Filtering movie sessions by date and movie.
5. Pagination implemented.
6. Admin panel `/admin/`.
7. Documentation is located at: `api/doc/swagger/`

### To run this project locally:

To run this projects locally, use the following steps:

1. Clone repo from GIT:

`git clone git@github.com:natalie-goriela/Cinema-API.git`

2. If you are using PyCharm - it may propose you to automatically create venv for your project 
and install requirements in it, but if not: 

```python
python -m venv venv
venv\Scripts\activate (on Windows)
source venv/bin/activate (on macOS)
pip install -r requirements.txt
```

3. Run the migrations:

`python manage.py migrate`

### Access:

1. Create your own user via: `/api/user/register/` 
2. Get access token via: `/api/user/token/`

###  To run project with docker:

1. `docker-compose build`
2. `docker-compose up`

### Environment variables:

The secret key to this project is saved within .env file, which is hidden.
You can create your own `.env` file to store your `SECRET_KEY` and other environment 
variables like it is shown in `.env_sample` file.
