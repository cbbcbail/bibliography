# [Annotated Bibliography of Tabular Visualization](https://pages.graphics.cs.wisc.edu/Tables/)

This repository contains an annotated bibliography of literature related to estimation in visualization. The literature is organized into categories and sorted by date of publication within categories. A short summary, and notes about how the work relates to - and is interesting or important to - our particular interests is followed by a citation in IEEE format. The author and year are emphasized for easy lookup and the DOI links are provided.

## Generating the Annotated Bibliography

The annotated bibliography is automatically compiled using `pandoc` and mdBook from Markdown and BibTex files. I use a Zotero collection to organize the works and export them to BibTex. The CSL file `ieee.csl` defines the IEEE citation style using citation style language and is modified to include the full bibliographic citation in text. The YAML file `mdbook.yml` is a GitHub Actions file that builds and deploys the annotated bibliography as an mdBook on the web. The file `book.toml` contains the metadata for mdBook and `src/SUMMARY.md` contains organizes the Markdown files for the mdBook page.

## Adding and Modifying the Bibliography

A good process for modifying the bibliography would be as follows. Clone the repository and load the existing works into a Zotero collection using the BibTex file. Add any additional works to the Zotero collection. Export the Zotero collection to BibTex to generate `Tables.bib`. Add notes to the `.md` files and use the format `[@cite]` to cite a work from the BibTex file. Push the changes to the BibTex and Markdown files to the repository and the updates will be automatically built and deployed.
