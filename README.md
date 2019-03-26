### sixpack
---
https://github.com/sixpack/sixpack

```js
require 'sixpack'

session = Sixpack::Session.new

session.participate("test", ["alt-1", "alt-2"])

session.convert("test")
```

```
pip install sixpack
SIXPACK_CONFIG=<path to config.yml> sixpack

gunicorn --access-logfile - -w 8 --worker-class=gevent sixpack.server:start
gunicorn --access-logfile - -w 2 --worker-class=gevent sixpack.web:start

cors_origins: *
cors_headers: ...
cors_credentials: true
cors_methods: GET
cors_expose_headers: ...

curl http://localhost:5001/experiments.json
curl http://localhost:5001/experiments/bule-or-red-header.json
```

```
{
  status: "ok",
  alternative: {
    name: "red"
  },
  experiment: {
    name: "button_color"
  },
  client_id: "xxx"
}
```


