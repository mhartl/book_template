# Book template

This is the $\mathrm{\LaTeX}$ book template I ([Michael Hartl](https://www.michaelhartl.com/)) use for writing books and other long-form documents (such as notes, problem sets, etc., for my [math learning project](https://www.michaelhartl.com/math-learning-project)). It is based on the template [generated](https://manual.softcover.io/book/polytex_tutorial) by the [Softcover system](https://github.com/softcover/softcover) (of which I am the principal author; although the hosting service has been shut down post-[acquisition](https://news.learnenough.com/big-news-about-learn-enough), the open-source project is still maintained).

Please feel free to clone the template and adapt it for your own uses. By design, the template can be converted to PDF using a plain `xelatex` command, but it's best when used with the `softcover` command:

```
$ softcover build:pdf --once
```

or, in abbreviated notation,

```
$ sc build:pdf -o
```
This generates a PDF and puts it in the `ebooks/` directory. See the [Softcover manual](https://manual.softcover.io/book) and especially the [installation instructions](https://manual.softcover.io/book/getting_started#sec-installing_softcover) for more.

I especially recommend running a Softcover server in a separate tab using

```
$ softcover server --pdf
```

This automatically builds a new PDF when the source files are changed. It's especially convenient when combined with a PDF reader like [Skim](https://skim-app.sourceforge.io/) that can auto-reload the document when the PDF changes. (To configure this, go to Skim > Preferences, click Sync, and select "Check for file changes".)

The file `latex_styles/custom.sty` includes a large number of commands that I've found useful when typesetting mathematics. Adapt it to your own uses as you see fit, or delete its contents entirely.

