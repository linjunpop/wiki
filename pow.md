# Conventions

1. A script `bin/setup` to setup a project. (Install dependency, initial db, seed data, etc.)
2. Same database account for dev/test env.
3. Same user account for dev env.
4. Use foreman as process manager, run all required processes with `foreman start`
5. Pow as proxy server.

Ref:

1. http://robots.thoughtbot.com/post/40110176152/foreman-as-process-manager-pow-as-dns-server-and-http
2. http://robots.thoughtbot.com/post/41439635905/bin-setup
