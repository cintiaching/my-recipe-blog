# my-recipe-blog
A toy project to pick up Django and React.

Following ["Django 5 by Example"](https://github.com/PacktPublishing/Django-5-By-Example) and online tutorials.

## Setup
Note for myself to remember how to set up from scratch.

### React
- Creating a Vite project
    ```
  npm create vite@latest
  ```
  Input the name of the project `my-recipe-frontend`, select `React`, then `TypeScript`

- then run
  ```
  cd my-recipe-frontend
  npm install
  npm run dev
  ```

### Django

This will create a Django project with the name my_recipe_backend.
```shell
django-admin startproject my_recipe_backend
```

Applying initial database migrations
```shell
cd my_recipe_backend
python manage.py migrate
```

Start the development server by typing the following command in the shell prompt
```shell
python manage.py runserver
```

Creating an application, Run the following command in the shell prompt from the project’s root directory
```shell
python manage.py startapp blog
```
This will create the basic structure of the application,
These files are as follows:
- `__init__.py`: This is an empty file that tells Python to treat the blog directory as a Python
module.
- `admin.py`: This is where you register models to include them in the Django administration
site—using this site is optional.
- `apps.py`: This includes the main configuration of the blog application.
- `migrations`: This directory will contain database migrations of the application. Migrations
allow Django to track your model changes and synchronize the database accordingly. This
directory contains an empty `__init__.py` file.
- `models.py`: This includes the data models of your application; all Django applications need to
have a `models.py` file but it can be left empty.
- `tests.py`: This is where you can add tests for your application.
- `views.py`: The logic of your application goes here; each view receives an HTTP request, processes
it, and returns a response.
With the application structure ready, we can start building the data models for the blog.



## Online Resources
In case I want to read them again

- https://blog.logrocket.com/build-react-typescript-app-vite/#creating-vite-project
