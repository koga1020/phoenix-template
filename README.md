# Phxdock

docker-compose for phoenix project.

## setup

```
$ git clone git@github.com:koga1020/phxdock.git some_app
$ cd some_app
$ rm -rf .git
$ mv env-example .env
$ echo "dotenv" > .envrc

# create project
$ mix phx.new . --app some_app

# set COMPOSE_PROJECT_NAME to the same as the mixproject name.
$ vim .env 
$ direnv allow

$ docker-compose up -d
```

after `mix phx.new`, update .gitignore.

```console
$ echo ".env" >> .gitignore
$ echo ".envrc" >> .gitignore
$ echo $DATA_PATH_HOST >> .gitignore
```
