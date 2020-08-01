# Phxdock

docker-compose for phoenix project.

## setup

```
$ git clone git@github.com:koga1020/phxdock.git .
$ mv env-example .env
$ echo "dotenv" > .envrc
$ direnv allow
```

after `mix phx.new`, update .gitignore.

```console
$ echo ".env" >> .gitignore
$ echo ".envrc" >> .gitignore
$ echo $DATA_PATH_HOST >> .gitignore
```
