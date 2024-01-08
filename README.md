# Understanding Tables

This repository contains an annotated bibliography of literature related to tabular visualization contained in `AnnotatedBibliography.md`. The literature is organized into categories and sorted by date of publication within categories. A short summary in one to two sentences and notes about how the work relates to and is interesting or important to our particular interests is followed by a citation in IEEE format. The author and year are emphasized for easy lookup and the DOI links are provided.

## Generating the Annotated Bibliography

The annotated bibliography is compiled using `pandoc` from a Zotero collection which is exported to BibTex and a markdown file `AnnotatedBibliographyRaw.md`. The command

```
pandoc -t markdown_strict --citeproc AnnotatedBibliographyRaw.md -o AnnotatedBibliography.md
```
is used to generate the annotated bibliography from the raw markdown and `Tables.bib` BibTex file. The CSL file `ieee.csl` defines the IEEE citation style using citation style language and is modified to include the full bibliographic citation in text.

## Adding and Modifying the Bibliography

The process for modifying the bibliography should be as follows. Load the collection into Zotero to add works to the collection. Export the Zotero collection to BibTex to generate `Tables.bib`. Add notes to the `AnnotatedBibliographyRaw.md` file and use the format `[@cite]` to cite a work from the BibTex file. The `pandoc` command listed above will fill in the IEEE citation in place of the citation tag when generating the final `AnnotatedBibliographyRaw.md` file.
