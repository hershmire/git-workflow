---
title: Dynamic Pages
---

# Dynamic Pages

Middleman has the ability to generate pages which do not have a one-to-one relationship with their template files. What this means is that you can have a single template which generates multiple files based on variables. Here's an example `config.rb` setup:

I removed a block of text in Topic 4.

## Arbitrary Ignores

It is also possible to ignore arbitrary paths when building a site using the new `ignore` method in your `config.rb`:

    ignore "/ignore-this-template.html"

You can give ignore exact source paths, filename globs, or regexes.

Haha, you are weird.

Topic1 change 1.

Topic2 change 2.

Master change 1.

Topic4 change 1.

Topic 5 change 1.

Topic 5 change 2.
