# heroku-buildpack-swig-lib

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that
allows you to set the SWIG_LIB environment variable correctly for installing e.g. M2Crypto.

Use together with `heroku-buildpack-apt` to install `swig`:

```
$ heroku buildpacks:set https://github.com/tiwilliam/heroku-buildpack-swig-lib.git
$ heroku buildpacks:set https://github.com/heroku/heroku-buildpack-apt.git
```

Install swig in `Aptfile`:
```
swig
```

## License

MIT
