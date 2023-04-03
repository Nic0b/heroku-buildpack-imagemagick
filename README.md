# heroku-buildpack-imagemagick

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for
vendoring the ImageMagick binaries into your project.

## Usage

In your project root:

```
heroku buildpacks:add https://github.com/steeple-org/heroku-buildpack-imagemagick --index 1
```

Now, you may configure ImageMagick by writing some config files in the `<your
app>/config/magick/*` directory.

## Upgrading

Go to https://github.com/steeple-org/imagemagick-bin/ to find
precompiled releases. Edit `bin/compile` accordingly, push, and redeploy the app.
