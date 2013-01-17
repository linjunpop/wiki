# Pow

## With Foreman

http://robots.thoughtbot.com/post/40110176152/foreman-as-process-manager-pow-as-dns-server-and-http

In `Procfile`

```ruby
web: bundle exec puma -p $PORT
```

Configure Foreman to always use the same port:

```bash
$ cd /path/to/myapp
$ echo “port: 7000” > .foreman
```

Relate the port to Pow:

```bash
$ echo 7000 > ~/.pow/`basename $PWD`
```
