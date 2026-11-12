# Beamer Documentation

## 1. Introduction
Beamer is a LaTeX document class used to create professional presentations, slides, and academic seminars.

## 2. Basic Structure

```latex
\documentclass{beamer}
\title{My Presentation}
\author{Student Name}
\date{\today}

\begin{document}
\begin{frame}
\titlepage
\end{frame}

\begin{frame}{Introduction}
Welcome to my presentation!
\end{frame}
\end{document}
```

## 3. Creating Slides and Lists

The `frame` environment is used to create slides.

```latex
\begin{frame}{Topics}
\begin{itemize}
    \item Introduction
    \item Objectives
    \item Conclusion
\end{itemize}
\end{frame}
```

- `itemize`: Creates bullet lists.
- `enumerate`: Creates numbered lists.

## 4. Themes and Colours

Themes customise the appearance of presentations.

```latex
\usetheme{Madrid}
\usecolortheme{default}
```

Common themes: Madrid, Berlin, Warsaw, Copenhagen and Singapore.

## 5. Adding Images

The `graphicx` package is used to insert images.

```latex
\usepackage{graphicx}

\begin{frame}{Image}
\centering
\includegraphics[width=0.5\textwidth]{image.png}
\end{frame}
```

## 6. Tables and Equations

Beamer supports tables and mathematical expressions.

```latex
\begin{frame}{Example}
\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Aman & 90 \\
\hline
\end{tabular}

\[
a^2+b^2=c^2
\]
\end{frame}
```

## 7. Overlays and Animations

Overlays display slide content gradually.

```latex
\begin{frame}{Steps}
First Point
\pause
Second Point
\pause
Third Point
\end{frame}
```

Using overlay specifications:

```latex
\begin{itemize}
\item<1-> First Point
\item<2-> Second Point
\end{itemize}
```

## 8. Columns and Blocks

Columns arrange content side by side, while blocks highlight important information.

```latex
\begin{frame}{Layout}
\begin{columns}
\column{0.5\textwidth}
Left Content

\column{0.5\textwidth}
Right Content
\end{columns}

\begin{block}{Definition}
Important Information
\end{block}
\end{frame}
```

Other blocks include `alertblock` and `exampleblock`.

## 9. Hyperlinks and Navigation

```latex
\hyperlink{slide2}{Go to Slide 2}

\begin{frame}[label=slide2]{Second Slide}
Welcome!
\end{frame}
```

Hide navigation symbols:

```latex
\setbeamertemplate{navigation symbols}{}
```

## 10. Conclusion

Beamer is a useful tool for creating structured presentations using LaTeX. It supports themes, images, equations, tables, overlays, and customised slide layouts.