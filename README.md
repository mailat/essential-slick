# Essential Slick

[![Build Status](https://travis-ci.org/underscoreio/essential-slick.svg?branch=3.3)](https://travis-ci.org/underscoreio/essential-slick)

[slick]: http://slick.lightbend.com
[download]: https://underscore.io/books/essential-slick/
[ebook-template]: https://github.com/underscoreio/underscore-ebook-template
[mdoc]: https://scalameta.org/mdoc/

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">Essential Slick</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://underscore.io" property="cc:attributionName" rel="cc:attributionURL">Richard Dallaway, Jonathan Ferguson, Underscore Consulting LLP</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

## Overview

Essential Slick is a book to get you started building application using the [Slick] database library.
It is aimed at Scala developers who need to become productive with Slick quickly.

It follows a tutorial style and includes exercises.

## Download

You can download the PDF, EPUB, and HTML formats of
this book for [free from the book web page][download].

## Table of Contents

  1. Basics

  2. Selecting Data

  3. Creating and Modifying Data

  4. Action Combinators and Transactions

  5. Data Modelling

  6. Joins and Aggregates

  7. Plain SQL

  A. Using Different Database Products

  B. Solutions to Exercises

## Building the Book

This book uses [Underscore's ebook build system][ebook-template].

The simplest way to build the book is to use [Docker Compose](http://docker.com):

- install Docker Compose; and
- run `go.sh` (or `docker-compose run book bash` if `go.sh` doesn't work).

This will open a `bash` shell running inside the Docker container which contains all the dependencies to build the book. From the shell run:

- `mkdir dist`
- `npm install`; and then
- `./sbt.sh`.

Within `sbt` you can issue the commands `pdf`, `html`, `epub`, or `all` to build the desired format(s) of the book. 

When you build the book, you'll see `Unknown link` warning messages.
You can ignore these (and if anyone wants to find out why they happen, do go for it).

The results are placed in the `dist` directory.


## Writing

- Essential Slick uses [mdoc] to check the Scala code on the book.
- The source files are in `src/pages`.
- The converted sources are output to `target/pages`.


