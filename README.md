`omd`
=====

Short description
-----------------

`omd` implements a Markdown frontend in OCaml (with no external
dependencies).

If you build the binary, `omd`, then you have a
[Markdown](http://daringfireball.net/projects/markdown/syntax) to HTML
converter.

An extensible Markdown-parser library is represented in `src/omd.ml`
and `src/omd.mli`.

`omd` hopefully implements the ["original Markdown
specs"](http://daringfireball.net/projects/markdown/syntax) with a few
Github Flavour Markdown characteristics.

Dependencies
------------

`omd` has been developed using OCaml 4.00.1. It is the only
dependency. (It should work with OCaml 3.12.)


----------------

Usage
-----

- to install `omd` using opam

   `opam install omd`

- to get the latest version of omd

  `git clone git@github.com:pw374/omd.git`

- to compile `omd`
  - using `oasis` and `ocamlbuild`

      `cd omd && make`

  - without `oasis`

      `cd omd/src && make`


----------------

N.B. You probably need to know markdown first if you plan on reading
the parser's source code. This implementation was driven mainly by two
things: the original Markdown syntax documentation
(<http://daringfireball.net/projects/markdown/syntax>) and
try-and-see-what-it-produces on
<https://github.com/pw374/sandbox>. Also, I used Pandoc to check its
behaviour sometimes. Now I can say than Pandoc does not really support
Github flavour Markdown even if it pretends to do so.

