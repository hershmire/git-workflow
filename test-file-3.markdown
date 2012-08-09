---
title: Dynamic Pages
---

# Dynamic Pages

Middleman has the ability to generate pages which do not have a one-to-one relationship with their template files. What this means is that you can have a single template which generates multiple files based on variables. Here's an example `config.rb` setup:

    :::ruby
    ["tom", "dick", "harry"].each do |name|
      page "/about/#{name}.html", :proxy => "/about/template.html" do
        @person_name = name
      end
    end

When this project is built, four files will be output:

Now, only the `about/tom.html`, `about/dick.html` and `about/harry.html` files will be output.

## Arbitrary Ignores

It is also possible to ignore arbitrary paths when building a site using the new `ignore` method in your `config.rb`:

    ignore "/ignore-this-template.html"

You can give ignore exact source paths, filename globs, or regexes.

Haha, you are weird.
