# Beamer Documentation

## 1. Introduction

Beamer is a LaTeX document class used to create presentations and slides. It helps create structured presentations using LaTeX commands.

## 2. Basic Structure

```latex
\documentclass{beamer}

\usetheme{Madrid}

\title{Introduction to LaTeX}
\author{Student Name}
\institute{Course Name}
\date{\today}

\begin{document}
\end{document}
```

- `\documentclass{beamer}`: Creates a presentation.
- `\usetheme{Madrid}`: Applies the Madrid theme.
- `\title{}`: Defines the presentation title.
- `\author{}`: Specifies the author.
- `\institute{}`: Specifies the course or institution.
- `\date{}`: Sets the presentation date.

## 3. Creating Slides

The `frame` environment is used to create individual slides.

```latex
\begin{frame}{What is LaTeX?}
LaTeX is a document preparation system.
\end{frame}
```

- `\begin{frame}`: Starts a slide.
- `\end{frame}`: Ends a slide.
- `\titlepage`: Displays the title slide.

## 4. Adding Bullet Points

The `itemize` environment creates unordered lists.

```latex
\begin{frame}{Features of LaTeX}

\begin{itemize}
    \item Academic Papers
    \item Research Articles
    \item Technical Reports
    \item Mathematical Equations
\end{itemize}

\end{frame}
```

- `\item`: Adds an individual bullet point.
- `itemize`: Creates a bullet-point list.

## 5. Text Formatting and Alignment

Beamer supports different text formatting commands.

```latex
\Large Large Text

\textbf{Bold Text}

\texttt{Typewriter Text}

\begin{center}
Centered Text
\end{center}
```

### Vertical Spacing

```latex
\vspace{0.5cm}
```

This adds vertical space between content.

## 7. Conclusion

Beamer makes it easy to create academic presentations using LaTeX. It supports themes, slides, bullet points, and text formatting.