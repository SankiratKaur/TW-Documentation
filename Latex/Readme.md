# LaTeX Documentation

## 1. Introduction
LaTeX is a document preparation system used to create professional documents, especially academic reports, research papers, and mathematical content.

## 2. Basic Structure

```latex
\documentclass[12pt,a4paper]{article}

\usepackage{amsmath}

\begin{document}
Hello World!
\end{document}
```

- `\documentclass`: Defines document type.
- `\usepackage`: Includes additional packages.
- `\begin{document}`: Starts the document.
- `\end{document}`: Ends the document.

## 3. Packages in LaTeX

Packages provide additional features and formatting options.

| Package | Purpose |
|---|---|
| `amsmath` | Mathematical equations |
| `graphicx` | Inserting images |
| `xcolor` | Adding colours |
| `geometry` | Page margins |
| `fontspec` | Font selection |
| `makeidx` | Creating an index |
| `fancyhdr` | Headers and footers |

Example:

```latex
\usepackage{amsmath}
\usepackage{graphicx}
\usepackage{xcolor}
```

## 4. Text Formatting

```latex
\textbf{Bold Text}
\textit{Italic Text}
\underline{Underlined Text}
\texttt{Monospaced Text}
```

Font sizes include `\small`, `\large`, `\Large`, `\huge` and `\tiny`.

## 5. Lists and Enumeration

### Unordered List

The `itemize` environment creates bullet-point lists.

```latex
\begin{itemize}
\item First Point
\item Second Point
\item Third Point
\end{itemize}
```

### Ordered List

The `enumerate` environment creates numbered lists.

```latex
\begin{enumerate}
\item First Point
\item Second Point
\item Third Point
\end{enumerate}
```

## 6. Mathematical Equations

```latex
\[
x^2+y^2=z^2
\]

\[
\frac{a+b}{c+d}
\]

\[
\sqrt{x^2+y^2}
\]
```

## 7. Matrices and Arrays

### Matrix

```latex
\[
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
\]
```

Other matrix environments include `matrix`, `pmatrix` and `vmatrix`.

### Array

```latex
\[
\begin{array}{|c|c|}
\hline
A & B \\
\hline
1 & 2 \\
\hline
\end{array}
\]
```

Column alignment: `l` (left), `c` (centre), `r` (right).

## 8. Tables

```latex
\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Aman & 90 \\
Riya & 95 \\
\hline
\end{tabular}
```

- `&`: Separates columns.
- `\\`: Starts a new row.
- `\hline`: Adds a horizontal line.
- `\multicolumn`: Combines columns.

## 9. Figures and Images

The `graphicx` package is used to insert images.

```latex
\usepackage{graphicx}

\begin{figure}[h]
\centering
\includegraphics[width=0.5\textwidth]{image.png}
\caption{Sample Image}
\label{fig:sample}
\end{figure}
```

## 10. Colours

The `xcolor` package is used to add colours.

```latex
\usepackage{xcolor}

\textcolor{red}{Hello World}

\colorbox{yellow}{Highlighted Text}
```

## 11. Bibliography

Bibliography is used to list the sources referred to in a document.

```latex
\bibliographystyle{plain}
\bibliography{references}
```

The `\cite{}` command is used to cite a reference stored in a `.bib` file.

## 12. Sections and Document Organisation

```latex
\section{Introduction}
\subsection{Background}
\subsubsection{Details}
```

Other useful commands:

- `\title{}`: Sets document title.
- `\author{}`: Specifies author.
- `\date{}`: Sets date.
- `\maketitle`: Displays title information.
- `\tableofcontents`: Generates a table of contents.

## 13. Special Characters

Some characters require a backslash to display correctly.

| Character | Command |
|---|---|
| % | `\%` |
| $ | `\$` |
| & | `\&` |
| # | `\#` |
| _ | `\_` |
| { } | `\{ \}` |

## 14. Fonts and Spacing

```latex
\setlength{\parindent}{1cm}

This is the first line.\\
This is the second line.
```

For font selection using XeLaTeX:

```latex
\usepackage{fontspec}
\setmainfont{DejaVu Serif}
```