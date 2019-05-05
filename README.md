# simple

A simple no build website. This website could just be in master, but in this example we are going to push it to the `gh-pages` branch.

## Debug

To debug that your simple website works run the following command to serve the current working directory:

```sh
python -m SimpleHTTPServer 3000
```

## Deploy

Install a tool that helps you push a directory to gh-pages

```sh
npm i -g push-dir
```

Use it to push the current directory to `gh-pages`. This command will push the current directory (`.`) to `gh-pages` and overwrite anything that is there already.

```sh
push-dir --dir=. --branch=gh-pages --cleanup
```
