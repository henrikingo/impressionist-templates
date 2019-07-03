# impressionist-templates
Templates to create [impress.js](https://github.com/henrikingo/impress.js) presentations from.
Used also by the [Impressionist creator](https://github.com/henrikingo/impressionist).

## Usage

    git clone --recursive https://github.com/henrikingo/impressionist-templates.git
    cp -r --dereference impressionist-templates/empty-slides new-presentation

* Each directory is one impress.js presentation.
* The main presentation file is index.html
* In each presentation directory, `impress.js` is a symlink to the actual `../impress.js`
  * Use `cp --dereference` when copying a template to your own presentation. This will give you a real impress.js directory embedded in the new presentation instead of empty symlink.
  * Probably won't work on Windows, but just copy the real impress.js dir into your presentation.
* impress.js is a git submodule, the actual impress.js repo

## About presentations in this repository

Impressionist-templates is intended to provide a collection of impress.js presentations that
can be used to create presentations with Impressionist. It only includes impress.js presentations
that actually work and can be edited in Impressionist.

Impressionist only supports a subset of all impress.js plugins. For example, only absolute
positioning works for now. Therefore the popular classic-slides demo is not found here.
