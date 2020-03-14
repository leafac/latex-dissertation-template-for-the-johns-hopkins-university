# [LaTeX](https://www.latex-project.org) Dissertation Template for the [Johns Hopkins University](https://www.jhu.edu)

[**Source**](https://github.com/leafac/latex-dissertation-template-for-the-johns-hopkins-university)

This is a LaTeX template that conforms to the [Formatting Requirements](https://www.library.jhu.edu/library-services/electronic-theses-dissertations/formatting-requirements/) given by the Johns Hopkins University Library.

**Disclaimer:** This template is here to help but offers no guarantees. You’re still responsible for ensuring that your dissertation conforms to the requirements.

## Compiling

Run [`latexmk`](https://ctan.org/pkg/latexmk):

```
$ latexmk
```

The generated PDF will be at [`dissertation.pdf`](dissertation.pdf).

## Contents

<details>
<summary><code>dissertation.tex</code>: Main Document</summary>

### PDF/A

https://www.pdf-online.com/osa/validate.aspx

</details>

<details>
<summary><code>dissertation.bib</code>: Bibliography</summary>

```bib
@misc{template,
  author = "Leandro Facchinetti",
  title = "{LaTeX} {Dissertation} {Template} for the {Johns} {Hopkins} {University}",
  howpublished = "\url{https://github.com/leafac/latex-dissertation-template-for-the-johns-hopkins-university}",
  note = "Accessed 2020-03-13"
}
```

In this file we include information about the citations. The existing content is just an example of an entry. For more on managing a bibliography, refer to the [BibTeX](https://ctan.org/pkg/bibtex) documentation. Or use a citation manager such as [Zotero](https://www.zotero.org) or [BibDesk](https://bibdesk.sourceforge.io), which produce a `.bib` file.

</details>

<details>
<summary><code>dissertation.xmpdata</code>: PDF/A Metadata</summary>

```latex
\Title{!!TODO!!}
\Author{!!TODO!!}
\Language{!!TODO, FOR EXAMPLE, “en-US”!!}
\Keywords{!!TODO!!\sep !!TODO!!\sep ...}
\Subject{!!TODO!!}
```

In this file we configure the metadata associated with the PDF (see the discussion about PDF/A in the section about `dissertation.tex` above). You may inspect some of the metadata using Preview in macOS by going to **Tools > Show Inspector**:

<p align="center">
<img alt="Metadata in Preview" src="docs/metadata.png" width="366" />
</p>

For more information, including other fields that you may configure in this file, refer to the documentation for the [`pdfx` package](https://ctan.org/pkg/pdfx).

</details>

<details>
<summary><code>.latexmkrc</code>: <code>latexmk</code> Configuration</summary>

```
$pdf_mode = 1;
```

Configure [`latexmk`](https://ctan.org/pkg/latexmk) to produce a PDF using the [`pdflatex`](https://ctan.org/pkg/pdftex) executable, instead of the default which is to produce a DVI using the `latex` executable.

</details>

## Beyond

TODO

## Related Work

The [Johns Hopkins University Library](https://www.library.jhu.edu/library-services/electronic-theses-dissertations/formatting-requirements/) mentions [this other LaTeX template](https://github.com/jrclayton/jhu-dissertation-mwe). What makes our template different is that it’s small and comes with [line-by-line explanations](#contents).
