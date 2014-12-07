reveal.js containerized
===
Just run a container with slides in `index.html`:

```bash
$ docker run --rm -v "$(pwd)/index.html:/revealjs/index.html" -p 8001:8000 calvingiles/revealjs
```

or markdown formated `slides.md`:

```bash
$ docker run --rm -v "$(pwd)/slides.md:/revealjs/slides.md" -p 8001:8000 calvingiles/revealjs
```

then navigate to port `8001` to see your slides.

Don't forget, you can get pdf output by adding `/?print-pdf` directly after the port in chrome and printing to pdf.
