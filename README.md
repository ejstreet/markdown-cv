# markdown-cv

A curriculum vitae maintained in plain text and rendered to HTML and PDF using CSS.

For more details, see the [original project](http://elipapa.github.io/markdown-cv), or the blog post on ['why I switched to markdown for my CV'](http://elipapa.github.io/blog/why-i-switched-to-markdown-for-my-cv.html) by [elipapa](https://github.com/elipapa).

***

## Distribution

To transform your plain text CV into a beautiful and shareable HTML page, you have two options:

### I. Use Github Pages to publish it online

1. Any change pushed to the `gh-pages` branch will trigger an update to the page.
3. Head to [cv.ejstreet.dev](https://cv.ejstreet.dev) to see the CV live.

### II. Build it locally and print a PDF

1. Clone this repo with the `git clone` command, and `cd` into it.
2. Run [jekyll](https://jekyllrb.com/) using `docker` with the command
```bash
docker run -it -p 4000:4000 -v $PWD:/srv/jekyll jekyll/jekyll:3.8 jekyll serve
```
3. The CV will be viewable at `http://localhost:4000`.
4. You can edit the `index.md` file and see the changes live in your browser.
5. To print a PDF, press <kbd>ctrl</kbd>/<kbd>⌘</kbd> + <kbd>p</kbd>. Print and web CSS media queries should take care of the styling.

## Styling

The included CSS will render the CV in using a modified version of the style by `davewhipp`, named `ejstreet`. The original styles are included for reference:

1. `kjhealy` the original default, inspired by [kjhealy's vita
template](https://github.com/kjhealy/kjh-vita).
2. `davewhipp` is a tweaked version of `kjhealy`, with bigger fonts and dates
  right aligned.  

To change the default style, simply change the variable in the
`_config.yml` file.

Any other styling is possible. More CSS style contributions and forks are welcome!

### Original Author

Eliseo Papa ([Twitter](http://twitter.com/elipapa)/[Github](http://github.com/elipapa)/[Website](https://elipapa.github.io)).

![Eliseo Papa](https://s.gravatar.com/avatar/eae1f0c01afda2bed9ce9cb88f6873f6?s=100)

### License

[MIT License](https://github.com/elipapa/markdown-cv/blob/master/LICENSE)
