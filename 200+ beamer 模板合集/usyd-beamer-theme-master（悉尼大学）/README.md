usyd-beamer-template
====================

This is an unofficial version of the University of Sydney presentation template
for use with beamer. It generally keeps to the intent of the official
presentation, however the most noticeable difference is the fonts.

The template has been tested in both the 4:3 and 16:9 aspect ratios, and should
work in any other.

How to use
----------

To add this theme to your presentation (assuming you are using git to version
control it as well), from the root directory you can add the repository as a
submodule

    git submodule add https://github.com/malramsay64/usyd-beamer-theme.git

To incorporate that directory into the path $\LaTeX$ searches add the following
before the `\usetheme` directive

    \makeatletter
    \def\input@path{{usyd-beamer-theme/}}
    \makeatother

Then using the theme is then as simple as adding the theme

    \mode<presentation>
    {%
        \usetheme{usyd}
    }

Customisation
-------------

The image in the titlegraphic is customisable using the
`\titlegraphic{<filename>}` command, where `<filename>` is the filename of the
image you want to use. The width of the image will always be half the slide
width. To prevent any issues with the image not filling he vertical height of
the slide there is a `\titlegraphicbackground{<colour>}` command which will
change the colour of the background to whichever colour you want, where
`<colour>` is a colour defined using the `\color{}` command. The default colour
is white.


Contributors
------------

Thanks to these people for their contributions

- [finnconor](https://github.com/finnconor)
