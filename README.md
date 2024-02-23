# labbcat-doc

Documentation, course materials, etc. for LaBB-CAT

These are HTML and PDF documents that can be browsed directly here:

<https://nzilbb.github.io/labbcat-doc/>

## Updating the documentation

The documentation is primarily a Quarto website.

Quarto project files are in the `site` directory, from where the site can be rendered:

```
cd site
quarto render
```

The site files, includeing HTML and PDF, are rendered into the `doc` directory.

## Website

Rendering of the live website is achieved using a GitHub Action, which is defined by:  
`.github/workflows/publish.yml`

In order to ensure changes are generated to the live site, simply commit changed .qmd files to GitHub, and the Action will automatically regenerate the website from them. This takes between 5 and 10 minutes to complete.

The rendered files are generated into a branch called `gh-pages`, and the repository is configured to host files from that branch.

The equivalent generation can be achieved manually using:

```
cd site
quarto publish gh-pages
```
