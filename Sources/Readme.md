New Namib GNU/Linux Homepage
======================

Source code of our new launch page for Namib GNU/Linux

## How to preview this on your local PC

* Install **hugo** on Namib with `yaourt -S hugo`
* clone this repository to your local pc with `https://github.com/meerkatbrowser/namib-website.git`
* change in the new dir with `cd namib-webiste`
* do a test run with `hugo server`
* preview the homepage with any webbrowser from `http://localhost:1313/public`

## How to preview this current version

* simply click on [here](https://namib.meerkat.tk/)

## How to develop this homepage further

* read the [Beginners Guide of Hugo](https://gohugo.io/overview/quickstart/) first
* modify the theme in [partials](https://github.com/meerkatbrowser/homepage/tree/gh-pages/themes/hugo-creative-theme/layouts/partials) and [static](https://github.com/manjaro/homepage/tree/gh-pages/themes/hugo-creative-theme/static) if needed
* edit the [config file](https://github.com/manjaro/homepage/blob/gh-pages/config.toml) to your needs
* run a preview on your local machine with `hugo server` from your **localhost**
* when satisfied run `hugo` to render the pages
* check **baseurl** in **public** and [change](https://github.com/manjaro/homepage/commit/8e3334067af2c5d40dc04eb402cf8100556b7fb3) if needed
* tell us about your fork

# Adding content

## Common problems

Due to HUGO's limitations, you cannot issue `hugo new`. The only way is to go to `content/support/commonproblems' and create a new entry manually (or just by copying and modifying an existing entry).

## Other content

Not all content can be easily extended. All pages are based on markdown files in the `content` directory. There are two types of content:

* "Dynamic" content
* "Static" content

"Static" content is content that heavily interacts with its base template. For example the template will only insert most of the content by itself and only take the content of the markdown file for some description.

"Dynamic" content will be created completely by the markdown file and is indicated by `type = "<anything>-post"`

# Translation

The homepage was designed to support translation. To translate the homepage, create a fork and edit the current language in `config.toml`. Also don't forget to modify the list of available languages and send your modifications upstream. Unfortunately there's no better way to create translations using HUGO.

All content was created to allow translation without skimming though the HTML templates. Just translate the entries in `config.toml` and all files in `content`.
