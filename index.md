# Markdown Test

This is a markdown test of Github. I'm wondering if I can just create a directory of markdown files, turn on Github hosting, and have it automatically convert those to HTML and host them (no Jekyl or anything else needed).

I've got a few questions.

1) Will md files be converted to HTML automatically?
2) Will gh serve readme.md, README.md, and index.md?
3) What order will gh serve those files?
4) How long does it take for gh-pages to generate?

That's about it. I think I already know how directories will work, etc.

Here are some answers about my questions above.

## Index

- [About](about)

## Automatic HTML

Github automatically converts markdown files to HTML. At the top of the page it puts a "title" with the name of the repo. That title links back to your home page. You can probably change this name with a yaml file or something.

Github uses Jekyll, behind the scenes, for this conversion. The [Jekyll Documentation](1) should provide information on how to configure things.

## Index Files

The following files will work as index filenames.

- index.md
- readme.md
- README.md

On a Mac you can't have both a `readme.md` and `README.md` in the same folder so there is no way to check which gets priority. The `index.md`, however, takes priority over both `readme.md` and `README.md` filenames.

## References

1: https://jekyllrb.com/docs/
