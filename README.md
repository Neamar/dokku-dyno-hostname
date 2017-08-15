# dokku-dyno-hostname

Sets the docker hostname option for dokku (https://github.com/dokku/dokku)

Currently just set `--hostname=app-name.dyno.scale`, for instance `myapp.web.1`

This is especially useful for monitoring services (esp. New Relic), that would other wise get a random hash as hostname for every container.


## requirements

- dokku 0.4.0+
- docker 1.8.x


## installation

```shell
# on 0.4.x
dokku plugin:install https://github.com/michaelshobbs/dokku-hostname.git dokku-hostname
```

## acknowledgement
This plugin is based on https://github.com/michaelshobbs/dokku-hostname
