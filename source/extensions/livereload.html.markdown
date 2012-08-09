---
title: LiveReload
---

# LiveReload

Middleman provides an official extension to support for the LiveReload browser extension. Simply install the gem:

    :::bash
    gem install middleman-livereload

If you have installed [the LiveReload extension] in your browser, you can have Middleman automatically tell the browser to refresh upon changes to your source code. To do this, you will need to start the Middleman server in LiveReload mode:

    :::bash
    middleman server --livereload

Now, browsers using the LiveReload extension can connect to Middleman and automatically refresh after you update your code.

[the LiveReload extension]: https://github.com/mockko/livereload#readme