# Sawmill UI

This is a collection of styles from my Sawmill WordPress theme. It is not a comprehensive UI, as I only write styles for UI I currently have implemented. This repo exists mostly as a quick way for me to copy these UI styles for my Github pages.

This is, of course, free for anyone to use. Over time, I may or may not make this UI collection more complete for general usage.

## Installation

To use Sawmill UI, copy the `core/` directory into the appropriate stylesheets asset directory in your project. Something like this:

```
$ cp -R core/ path/to/your/project/directory
```

Secondly, you will want to ensure that all the included Bower packages, [Shevy](https://github.com/kyleshevlin/shevy) and [Condo](https://github.com/kyleshevlin/condo) are installed. In the root directory of your project, do this:

```
$ bower install
```

This will install Shevy and Condo in the `bower_components/` directory. You may need to update the paths set in `sawmill_ui.scss` if your directory structure is different. Double check this.

Lastly, this is an uncompiled UI kit. That means you will need something to do the asset compilation. In this case, that means compiling Sass to CSS. Your project may do this automagically (such as if you're using Rails) or you may need to set up a process for this with something like [Grunt](https://github.com/gruntjs/grunt) or [Gulp](https://github.com/gulpjs/gulp). I cannot, in this README, walk you through how to set this up. If you would like an example, I suggest you look at my [Grunt Starter Kit](https://github.com/kyleshevlin/grunt-starter-kit) repo.

## Important Notes

Currently, the Sawmill UI utilizes two Google fonts. You may import them how you choose, or replace them all together. Currently, I simply link to them in the `<head>` of the document. Yes, I understand this adds a request to the page, but I'd rather use this than a CSS import.

Add the following to your `<head>`:

```html
<link href='https://fonts.googleapis.com/css?family=Droid+Serif:400,700|Catamaran:100,400,700' rel='stylesheet' type='text/css'>
```
