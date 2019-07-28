# LaTeX Learning
LaTeX code files, was written in my learning process.

[![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## What is LaTeX?
LaTeX is a **document preparation system** for high-quality typesetting. It is most often used for medium-to-large **technical** or **scientific** documents but it can be used for almost any from of publishing.

LaTeX encourages authors not to worry too much about the apprearance of their documents but not concertrante on getting the right content.

**What it is**, not **How it looks**.

## Why should I use LaTeX?
* Small files.
* Cross-platform compatibility
* Easy to make templates.
* Free.

## MS Word vs LaTeX
<img src="screenshots/latexvsword.png" width="350" alt="word vs latex">

## How does it work?
1. You write your document in plain text with commands that describe its structure and meaning.
2. The latex program processes your text and commands to produce a beautifully formatted document.

## Required Tools
* Compiler
  * Gnu/Linux (TexLive)
  * Mac (MacTex)
  * Windows (MIKTeX)
* Editor
  * TeXstudio, Texmaker, ...
* Or use web-based Online Editors
  * www.sharelatex.com
  * www.writelatex.com

## Get Started
* Typesetting
  * comment: `% this is comment`
  * new line: `\\`
  * spaces: `\quad` or `\qquad`
  * print %, {, ...and more: `\%`, `\{`, ... (use anti-slash before special character)
  * bold: `\textbf{value}`
  * italic: `\textit{value}`
  * underline: `\underline{value}`
  * 3 dots: `\dots`
* Math
  * inline math mode: `$ value $`
  * symbols: `\alpha`, `\beta`, `\omega`, ...
  * sub-script: `X_2`
  * sup-script: `X^2`
  * multi sub or sup script: `x^{2x + 3}` or `x_{2x + 3}` (use brackets)
  * merge between sub and sup script: `\sum_{k=1}^n`
  * fractional: `d=\frac{5x}{y}`
  * equation
  ```latex
     \begin{equation}
        \omega = \sum_{i=1}^{n}w_ix % content of equation
     \end{equation}
  ```
  * label in equation
  ```latex
     \begin{equation}
        \label{omega eq} % name of equation used to refered
        \omega = \sum_{i=1}^{n}w_ix
        \end{equation}
     \ref{omega eq}
   ```
* Lists
  * unordered list
  ```latex
     \begin{itemize} % Unordered list
        \item Stackoverflow
        \item GitHub
     \end{itemize}
  ```
  * unordered list
  ```latex
    \begin{itemize} % Unordered list
       \item Stackoverflow
       \item GitHub
    \end{itemize}
  ```
  * ordered list
  ```latex
    \begin{enumerate} % Ordered list
       \item HTML
       \item CSS
    \end{enumerate}
  ```
  * merge and list inside list
  ```latex
    \begin{enumerate} % list inside list
    \item HTML
       \begin{enumerate}
         \item HTML4
         \item HTML5
       \end{enumerate}
    \item CSS
    \item PHP
    \item JS framework
       \begin{itemize}
         \item Angular
         \item React
         \item Vue
       \end{itemize}
    \end{enumerate}
  ```
* Sections
  ```latex
    \section{Introduction}
    \label{intro section}
    This is the first section

    \section{Problematic}
    This section based on section \ref{intro section}
    \subsection{Problem of access}
    Just simple Text
    \subsubsection{Title here}
  ```
* Packages
  ```latex
    \documentclass{article}
    \usepackage{package_name} % add package
    \begin{document}
      Hello!
    \end{document}
  ```
* Package > amsmath
  ```latex
    \documentclass{article}
    \usepackage{amsmath} % use package (LaTeX will install package if not exist in your computer)
    \begin{document}
      \begin{equation*} % *: don't add number of equation
        \sum
    \end{equation*}

    \begin{align*} % align equation..
      (X+1)^3&=(X+1)(X+1)(X+1)\\
      &=(X+1)(X^2 + 2X + 1)\\
      &=X^3+3X^2+3X+1
    \end{align*}
    \end{document}

    \begin{equation} % for add single number of equation
    \begin{align*}
      (X+1)^3&=(X+1)(X+1)(X+1)\\
      &=(X+1)(X^2 + 2X + 1)\\
      &=X^3+3X^2+3X+1
    \end{align*}
    \end{equation}
  ```
