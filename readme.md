# Jekyll in a Docker container

This is [Jekyll](https://jekyllrb.com/) (a simple, blog-aware, static site generator)
installed in a Docker container.

## How to use it

```
docker build . -t jekyll
docker run --rm -it jekyll --help
```

or use an image from the docker hub:

```
docker run --rm -it gtrafimenkov/jekyll --help
```

## License

MIT
