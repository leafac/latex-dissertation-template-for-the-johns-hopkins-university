# [LaTeX](https://www.latex-project.org) Dissertation Template for the [Johns Hopkins University](https://www.jhu.edu)

[**Source**](https://github.com/leafac/latex-dissertation-template-for-the-johns-hopkins-university)

This is a minimal LaTeX template that conforms to the [Formatting Requirements](https://www.library.jhu.edu/library-services/electronic-theses-dissertations/formatting-requirements/) given by the Johns Hopkins University Library.

**Disclaimer:** This template is here to help but offers no guarantees. You’re still responsible for ensuring that your dissertation conforms to the requirements.

## Compiling

Run [`latexmk`](https://ctan.org/pkg/latexmk):

```console
$ latexmk
```

The generated PDF will be at [`dissertation.pdf`](dissertation.pdf).

## Contents

<details>
<summary><strong><code>dissertation.tex</code>: LaTeX Source</strong></summary>

### PDF/A

https://www.pdf-online.com/osa/validate.aspx

</details>

<details>
<summary><strong><code>dissertation.bib</code>: Bibliography Entries</strong></summary>

```bib
@misc{template,
  author = "Leandro Facchinetti",
  title = "{LaTeX} {Dissertation} {Template} for the {Johns} {Hopkins} {University}",
  howpublished = "\url{https://github.com/leafac/latex-dissertation-template-for-the-johns-hopkins-university}",
  note = "Accessed 2020-03-13"
}
```

This is just an example of a bibliography entry. For more on managing a bibliography, refer to the [BibTeX](https://ctan.org/pkg/bibtex) documentation. Or use a citation manager such as [Zotero](https://www.zotero.org) or [BibDesk](https://bibdesk.sourceforge.io), which produce a `.bib` file.

</details>

<details>
<summary><strong><code>dissertation.xmpdata</code>: PDF/A Metadata</strong></summary>

```latex
\Title{!!TODO!!}
\Author{!!TODO!!}
\Language{en-US}
\Keywords{!!TODO!!\sep !!TODO!!\sep ...}
\Subject{!!TODO!!}
```

See [§ PDF/A](#pdf-a). For more options, refer to the documentation of the [`pdfx` package](https://ctan.org/pkg/pdfx).

</details>

<details>
<summary><strong><code>.latexmkrc</code>: <code>latexmk</code> Configuration</strong></summary>

```perl
$pdf_mode = 1;
```

Configure [`latexmk`](https://ctan.org/pkg/latexmk) to produce a PDF using the [`pdflatex`](https://ctan.org/pkg/pdftex) executable, as opposed to producing a DVI using the `latex` executable.

</details>

## Beyond

TODO

## Related Work

The [Johns Hopkins University Library](https://www.library.jhu.edu/library-services/electronic-theses-dissertations/formatting-requirements/) mentions [a template by John “Randy” Clayton](https://github.com/jrclayton/jhu-dissertation-mwe). There’s a whole lineage of templates of that sort. What makes this template different is that it’s very small and comes with line-by-line explanations.
