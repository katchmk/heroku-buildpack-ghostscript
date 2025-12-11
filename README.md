# Heroku Buildpack for Ghostscript

Compiles and installs Ghostscript 10.06.0 on Heroku.

## Install

    # Use heroku-buildpack-ghostscript
    $ cd /path/to/your-app
    $ heroku buildpacks:add https://github.com/katchmk/heroku-buildpack-ghostscript

## Notes

- The first build will compile Ghostscript from source, which takes a few minutes
- Subsequent builds use a cached binary for faster deployment
- Ghostscript is installed to `$HOME/vendor/gs/bin/gs`
