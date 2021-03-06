# Readme

This is a markdown test of Github. I'm wondering if I can just create a directory of markdown files, turn on Github hosting, and have it automatically convert those to HTML and host them (no Jekyl or anything else needed).

I've got a few questions.

1. Will md files be converted to HTML automatically?
2. Will gh serve readme.md, README.md, and index.md?
3. What order will gh serve those files?
4. How long does it take for gh-pages to generate?

That's about it. I think I already know how directories will work, etc.

Here are some answers about my questions above.

## Index

- [About](about) - Linked to `about`
- [About](about.md) - Linked to `about.md`
- [More](more) - Linked to `more` directory

## Automatic HTML

Github automatically converts markdown files to HTML. At the top of the page it puts a "title" with the name of the repo. That title links back to your home page. You can change this with a `_config.yaml` file.

Github uses Jekyll, behind the scenes, for this conversion. The [Jekyll Documentation](1) should provide information on how to configure things.

## Index Files

The following files will work as index filenames.

- index.md
- readme.md
- README.md

On a Mac you can't have both a `readme.md` and `README.md` in the same folder so there is no way to check which gets priority. The `index.md`, however, takes priority over both `readme.md` and `README.md` filenames.

The `readme.md` file takes precedence on Github, which will allow you to write a separate readme for your Github audience than for your web audience.

## Links

If you link to an `.md` file, it will automatically.

Here are several options for linking to internal pages.

- Link to the md file (`about.md`)
- Link to a single word (`about`)
- Link to a directory (`more`)

If you link to `about` then it will appear in the uri as `yourdomain/about` but will display the html conversion version of the `about.md` file.

## Google Analytics

You can add Google Analytics to your pages by simply adding a line like the following to your _config.yml file.

`google_analytics: UA-xxxxxxx-xx`

## Includes

You can put something like `{&#37; include footer.html &#37;}` in your markdown files to include the file `_includes/footer.html`. This works to include html and markdown files.

## Observations

- Adding `name: Whatever` to the `_config.yaml` causes the site name not to show up at the top and link back
- Adding `title: Watever` to the `_config.yaml` brings back the site name and it's link to the index
- Adding `url: https://example.com` makes that the title link

## References

1: https://jekyllrb.com/docs/
