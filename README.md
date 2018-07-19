Set the config `YARN_TARGET` to specify what to build with yarn.

```
heroku buildpacks:add https://github.com/heroku/heroku-buildpack-nodejs#v83 -a myapp
heroku buildpacks:add https://github.com/revmischa/heroku-buildpack-yarn -a myapp
```

Will run `yarn $YARN_TARGET` on your application.

Useful if you want to build your application with webpack and then serve it up.
