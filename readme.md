# Dynamic Documents with R and knitr

In the very beginning, I planned to write this book with Markdown, but later
I changed my mind and wrote it in LyX instead. For those who are still
interested in the Markdown source, please see the [markdown](markdown)
directory.

Now this book has been published by Chapman & Hall:
<http://www.crcpress.com/product/isbn/9781482203530> You can also find it on
Amazon: <http://www.amazon.com/gp/product/1482203537>

## The book source

Besides the old Markdown source which is really only an empty sketch, this
repository also provides the real source files for the first three chapters
of the book, so that you can learn how the book was written and quickly get
started with writing books using the LaTeX style by Chapman & Hall.

The main file is `DDR-Yihui-Xie-Chap1-3.lyx`; the Rnw file
`DDR-Yihui-Xie-Chap1-3.Rnw` was exported from LyX; `krantz.cls` is the LaTeX
class provided by Chapman & Hall, and I wrote a simple LyX layout file
`krantz.layout`; `DDR-Yihui-Xie.bib` contains some bibliography entries, and
`DDR-packages.bib` is dynamically generated from **knitr** (see the last
chunk in the LyX or Rnw file).

The PDF of the first three chapters can be downloaded
[here :arrow_down:](https://bitbucket.org/stat/knitr/downloads/DDR-Yihui-Xie-Chap1-3.pdf).

If you do not use LyX, you can simply open the Rnw file and start from there.

Note I was using the tikz device for graphics in this book, and
unfortunately the **tikzDevice** package has been archived on CRAN for a
long time, so some users might find it difficult to install. In that case,
you can change the default device to `pdf`:

```s
opts_chunk$set(dev = 'pdf')  # or cairo_pdf
```

Be sure to read the session info in the preface because your R packages may
not be up-to-date to reproduce the PDF. Normally I use development versions
of my packages, because I often find little problems that I need to solve
for the book, and these changes will end up in the development versions.

## Contact

GitHub issues (<https://github.com/yihui/knitr-book/issues>) is the
preferred way for feedbacks. You can also reach me by email if you really
want:

```bash
echo oybuwycxy.trpb | tr bopcrbtucwxyc+ exmiaen@iyuih
```
