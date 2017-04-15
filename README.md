# heroku-buildpack-pandoc

A buildpack provides `pandoc` and `pandoc-citeproc`.

## install

```
heroku buildpacks:add https://github.com/uetchy/heroku-buildpack-pandoc.git
```

then you'll got buildpacks like this:

```
❯ heroku buildpacks
=== app Buildpack URLs
1. heroku/python
2. https://github.com/uetchy/heroku-buildpack-pandoc.git
```

## test

```
docker-compose run test
```
