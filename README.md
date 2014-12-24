# Beetle-Htmlmin

Minifies the HTML files in the [Beetle](https://github.com/cknv/beetle) output directory using the [htmlmin](https://github.com/mankyd/htmlmin) library.

When `beetle_htmlmin` has been added to the list of plugins in your Beetle `config.yaml` file, you can run `beetle htmlmin` to minify the HTML files in the output directory. It can also be done at the same time as the rendering of the site by running it as `beetle render htmlmin`.

You can specify arguments to htmlmin inside your `config.yaml` file by using the `args` object like this:

    plugins:
      - name: beetle_htmlmin
        args:
          remove_empty_space: True
          remove_comments: True
          remove_optional_attribute_quotes: False

A complete list of possible arguments and their default values can be found in the [htmlmin documentation](https://htmlmin.readthedocs.org/en/latest/reference.html).
