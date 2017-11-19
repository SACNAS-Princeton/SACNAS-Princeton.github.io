# SACNAS-Princeton Website

The SACNAS-Princeton website is built using [Jekyll](https://jekyllrb.com).
The current theme is the [Spectral](https://html5up.net/spectral) theme from HTML5 UP.

This README will explain the basics on how to add pages to the website and update existing ones.

## New Pages

New pages can be added easily. For example, to add a new page called `Foo`, you can do the following:

1. Create `foo.md` (if you want to use Markdown) or `foo.html` (if you want to use HTML)
2. Add the following header to the top of the page:
```
    ---
    layout: page
    title: Foo
    ---
```
A new item for `Foo` in the navigation menu will be created.
You can then add your content to the file you created after the header.

## Gallery

The gallery is heavily based off of [this](https://github.com/opieters/jekyll-image-gallery-example) example gallery in Jekyll using [Isotope](https://isotope.metafizzy.co) and [lightgallery](http://sachinchoolur.github.io/lightGallery/)

### Adding images to the Gallery

The following requires you to have cloned the repository on your computer and to have the required dependencies (namely Python and YAML) installed:

1. Put your images in the `gallery` directory
2. Execute the following (from the `_data` directory)
```
    python gallery_creator.py
```
This script will modify the `gallery.yml` file in the `_data` directory.

### Adding titles and captions to images
For this example, let's assume that you want to add the title/caption `Foo` to image `foo.jpg`
1. Open up the `gallery.yml` file in a text-editor
2. Find the line containing `filename: foo`
3. Underneath the line `thumbnail: foo-thumbnail.jpg`, add the following:
```
    title: Foo
```


   
