# Jupyter Book and Colab

One of the document production pipelines uses multiple times in Reconstrue 

Basicly, there was a pre-existing tool, called Jupyter Book, which can
take a repo full of `*.ipynb` and `*.md` files plus a table of
contents as input, and output a static HTML "book" of the input
Jupyter notebooks and Markdown files.


## Integrating the two

![]("./jupyter_book_to_colab.png")

Jupyter Book could be configured to provide links to MyBinder in what
the project calls an "Interact button." Simply hacking on some HTML
templates was enough to get the code to where it could link to Colab
instead.

## Detailed interaction sequence

In the general case it works as follows, which is confusing enough.

![]("./four_reps_of_ipynb.png")

Even more confusingly, in this case `foo.com` is github.io, the GitHub
Pages site, not github.com.

(GitHub Pages is a free service: a static website for any repos on
github.com. A.k.a. `gh-pages` branches back in the day.)

Note: Reconstrue has been transitioning away from using Jupyter Book,
and moving toward Gatsby tooling. There are posibilities that perhaps
they could play well together. The Jupter Book project lead has been
considering the same.
