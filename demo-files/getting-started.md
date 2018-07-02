---
title: 'Getting started'
order: 5
---
## On TUX machine

It is possible to build docs without installing anything. Just use our local network machine: `TUX-XPS-8500`. Simply follow these instructions:

1. Connect via ssh on your computer <br>`ssh -t tux@10.129.43.33 "cd ../../var/www/html/Jekyll-tests ; bash"`
    * Usual Kolor password.
2. Clone the GitHub repository to a custom folder name (`[my-doc-folder]` in this case) <br>`git clone git@github.com:KolorCompany/kds.git [my-doc-folder]`
3. Apply chmod <br>`sudo chmod 777 -R [my-doc-folder]`
    * Usual Kolor password.
4. Choose an export folder name (`[my-doc-export-folder]` in this case) and run <br>`jekyll build --source [my-doc-folder] --destination [my-doc-export-folder] --baseurl /Jekyll-tests/[my-doc-export-folder] --watch`
    * `--watch` option allows to auto generate each time a file is modified into the source.
7. Once built, you can browse your website `http://10.129.43.33/Jekyll-tests/[my-doc-export-folder]`
8. You can now directly edit your own content on samba local network `TUX-XPS-8500/Jekyll-tests/[my-doc-folder]/` by importing folder into your editor.

## Locally

1. Install [Jekyll](https://jekyllrb.com/docs/installation/) on your machine.
2. [Download documentation system](https://github.com/KolorCompany/kds/archive/master.zip) files.
3. Extract it to a folder, optionally delete `demo-files` folders to put your own content.
4. Configure your `config.yml` file to your needs.
5. Run command `$ jekyll build` from your project folder.
6. By default static website is generated into your project folder in a folder called `_site`. See [Jekyll basic usage](https://jekyllrb.com/docs/usage/) for more informations.

## On Github Pages

Here is an [example](https://kolorcompany.github.io/kds/) of a Jekyll generation powered by [GitHub Pages](https://pages.github.com/).

1. [Download documentation system](https://github.com/KolorCompany/kds/archive/master.zip) files.
2. Extract it to a folder, optionally delete `demo-files` folders.
3. Configure your local and remote git repository.
4. Follow instructions of [GitHub Pages](https://pages.github.com/).
