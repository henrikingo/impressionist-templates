# impressionist-templates
Templates to create [impress.js](https://github.com/henrikingo/impress.js) presentations from.
Used also by the [Impressionist creator](https://github.com/henrikingo/impressionist).

## Usage

    git clone --recursive https://github.com/henrikingo/impressionist-templates.git
    cd impressionist-templates

* Each directory is one impress.js presentation.
* The main presentation file is index.html
* impress.js is a git submodule, the actual impress.js repo
* In each presentation directory, `impress.js` is a symlink to the actual impress.js
  * Probably won't work on Windows, but the below steps will
* If you create a presentation out of a template:
  1. Create a copy of the template directory (e.g. `empty-slides`)
  2. Delete the symlink `impress.js`
  3. Copy the actual `impress.js` directory into its place (e.g. `empty-slides/impress.js`)
  4. Under `empty-slides/extras`, delete the extra modules you won't need, to save space.
     (e.g. `empty-slides/impress.js/extras/*`)

(Impressionist will use the above sequence when creating a new presentation from a template.)

## About presentations in this repository

Impressionist-templates is intended to provide a collection of impress.js presentations that
can be used to create presentations with Impressionist. It only includes impress.js presentations
that actually work and can be edited in Impressionist.

Impressionist only supports a subset of all impress.js plugins. For example, only absolute
positioning works for now. Therefore the popular classic-slides demo is not found here.