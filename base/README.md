# [LaTeX](https://www.latex-project.org) Dissertation Template for the [Johns Hopkins University](https://www.jhu.edu) · Base

This is a minimal LaTeX template that conforms to the [Formatting Requirements](https://www.library.jhu.edu/library-services/electronic-theses-dissertations/formatting-requirements/) given by the Johns Hopkins University Library.

**Disclaimer:** The template is here to help but offers no guarantees. You’re still responsible for ensuring that your dissertation conforms to the requirements.

# Compiling

Run [`latexmk`](https://ctan.org/pkg/latexmk):

```console
$ latexmk
```

The generated PDF will be at [`dissertation.pdf`](dissertation.pdf).

# LaTeX Source ([`dissertation.tex`](dissertation.tex))

## PDF/A

# Bibliography Entries ([`dissertation.bib`](dissertation.bib))

```bib
@misc{template,
  author = "Leandro Facchinetti",
  title = "{LaTeX} {Dissertation} {Template} for the {Johns} {Hopkins} {University}",
  howpublished = "\url{https://github.com/leafac/latex-dissertation-template-for-the-johns-hopkins-university}",
  note = "Accessed 2020-03-13"
}
```

This is just an example of a bibliography entry. For more on managing a bibliography, refer to the [BibTeX](https://ctan.org/pkg/bibtex) documentation. Or use a citation manager such as [Zotero](https://www.zotero.org) or [BibDesk](https://bibdesk.sourceforge.io), which produce a `.bib` file.

# PDF/A Metadata ([`dissertation.xmpdata`](dissertation.xmpdata))

```latex
\Title{!!TODO!!}
\Author{!!TODO!!}
\Language{en-US}
\Keywords{!!TODO!!\sep !!TODO!!\sep ...}
\Subject{!!TODO!!}
```

See [§ PDF/A](#pdf-a). For more options, refer to the documentation of the [`pdfx` package](https://ctan.org/pkg/pdfx).

# `latexmk` Configuration ([`.latexmkrc`](.latexmkrc))

```
$pdf_mode = 1;
```

Configure `latexmk` to produce a PDF using the [`pdflatex`](https://ctan.org/pkg/pdftex) executable, as opposed to producing a DVI using the `latex` executable.
