# LaTeX Documentation

## 1. Introduction
LaTeX is a document preparation system used to create professional documents, especially academic reports, research papers, and mathematical content.

## 2. Basic Structure

```latex
\documentclass[12pt,a4paper]{article}

\begin{document}
Hello World!
\end{document}
```

## 3. Text Formatting

```latex
\textbf{Bold Text}
\textit{Italic Text}
\underline{Underlined Text}
```

## 4. Mathematical Equations

```latex
\[
x^2+y^2=z^2
\]
```

## 5. Matrices

```latex
\[
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
\]
```

## 6. Tables

```latex
\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Aman & 90 \\
\hline
\end{tabular}
```

## 7. Figures and Images

```latex
\usepackage{graphicx}

\includegraphics[width=0.5\textwidth]{image.png}
```

## 8. Colours

```latex
\usepackage{xcolor}

\textcolor{red}{Hello World}
```

## 9. Bibliography

```latex
\bibliographystyle{plain}
\bibliography{references}
```

## 10. Other Important Concepts

- Special characters
- Arrays and display styles
- Page formatting and spacing
- Fonts
- Boxes and lines
- Indexing
- Sections and subsections