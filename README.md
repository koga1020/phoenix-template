# Phxdock

docker-compose for phoenix project.

## setup

```
$ git clone git@github.com:koga1020/phxdock.git some_app
$ cd some_app
$ rm -rf .git
$ mv env-example .env
$ echo "dotenv" > .envrc
$ direnv allow
$ mix phx.new . --app some_app
$ docker-compose up -d
```

after `mix phx.new`, update .gitignore.

```console
$ echo ".env" >> .gitignore
$ echo ".envrc" >> .gitignore
$ echo $DATA_PATH_HOST >> .gitignore
```
