# PHPStan docker image

## User
We are recommend to use the images as an shell alias to access via short-command. To use simply phpstan everywhere on CLI add this line to your ~/.zshrc, ~/.bashrc or ~/.profile.

```
alias phpstan='docker run --tty --rm --volume $PWD:/app jacquesndl/phpstan $*'
```

If you don't have set the alias, use this command to run the container:
```
docker run --tty --rm --volume /path/to/project:/app jacquesndl/phpstan [some arguments for PHPStan]
```

For example:
```
docker run --tty --rm --volume /path/to/project:/app jacquesndl/phpstan analyse .
```
