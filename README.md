# flightphp.com

This is the repository of the website [flightphp.com](http://flightphp.com).
The website is built with the program [Jekyll](https://jekyllrb.com/).

## Contributing

If you would like to make updates or add language translations, just fork
the `master` branch and submit a pull request. Do not fork the `gh-pages` branch
since that will only contain the compiled html from Jekyll.

## Translations

If you would like to translate the website into another language, follow these steps:

1. Create a new folder at the root level with the proper [ISO 639-1](http://www.loc.gov/standards/iso639-2/php/code_list.php)
code as the name. There should be an existing `en` folder for English.

2. Copy the contents of the `en` folder to your new folder. For example from `en` into `fr`.

3. In each of the `.html` files, there is a `lang` setting at the top. Change the value to your language code.

    ``` yaml
    layout: default
    lang: fr
    ```

4. Create a new folder in the `_includes` folder with your language code.
There should be an existing `_includes/en` folder for English.

5. Copy the contents of the `_includes/en` folder into your new folder. For example from `_includes/en` into `_includes/fr`.

6. Translate all the `.md` files. These files use the [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/) syntax.

7. Run the website through Jekyll, `jekyll serve --watch`.

8. Change the url to your language, `http://localhost:4000/fr/`.
