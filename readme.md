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

Example of serving a site locally:
- cd to your project
- `docker run --rm -it -p 4000:4000 -v $(pwd):/site gtrafimenkov/jekyll serve -s /site -H 0.0.0.0`
- open [http://127.0.0.1:4000/](http://127.0.0.1:4000/)

## License

MIT
