--

🎬 Start the Application (run commands)

⭐️ `docker-compose build`

🔹 When to use it:

✅ Run it when you change the Dockerfile or dependencies (e.g., requirements.txt).

✅ Before starting the project for the first time.

⭐️ `docker-compose up`

🔹 When to use it:

✅ Run it every time you want to start the application.

⭐️ `docker-compose down`

🔹 When to use it:

✅ When you want to fully stop and remove the containers.

✅ If you need a fresh restart of the project.

Common commands to be used:
`docker-compose -f docker-compose-deploy.yml down`

`docker-compose run --rm app sh -c "python manage.py makemigrations"  `

`docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"  `

`docker-compose run --rm app sh -c "python manage.py startapp xxxx"`

`docker-compose run --rm app sh -c "python manage.py  createsuperuser"`

`docker-compose build`

`docker-compose up`

`docker-compose down`

`docker-compose run --rm app sh -c "python manage.py test"`

`docker-compose run --rm app sh -c "flake8"`

`docker-compose run --rm app sh -c "isort ."`
