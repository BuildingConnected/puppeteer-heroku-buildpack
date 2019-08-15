# puppeteer-heroku-buildpack

Installs dependencies needed in order to run puppeteer on heroku. Be sure to include `{ args: ['--no-sandbox'] }` in your call to `puppeteer.launch`

## Usage

```sh-session
$ heroku buildpacks:add https://github.com/BuildingConnected/puppeteer-heroku-buildpack.git
```

Include `--app` to specify which app, and `--index` with a number value so you include this buildpack after the ones we already have installed.

See https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app for more.
