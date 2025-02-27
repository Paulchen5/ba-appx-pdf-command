# ba-appx-pdf-command

## Setup

To use `\baincludepdf` command put the file [`command.tex`](https://raw.githubusercontent.com/Paulchen5/ba-appx-pdf-command/main/command.tex) into your project directory. Afterwards input the file into your `main.tex` document with the following command: `\input{command.tex}`. The import has to be done before the `\begin{document}` statement.

## Usage
> [!WARNING]
> The given label of the pages looks like one of the following: `\label{appendix:\@bapdftitle:page:\theappxPageCounter}` or `\label{appendix:\@bapdflabel:page:\theappxPageCounter}`

## Example Usages
```tex
\baincludepdf[pages=1-3,label=myLabel,source=My Source]{file.pdf}{My Caption}
```
To reference page 2 of the exmplae use the following command:
```tex
\ref{appendix:myLabel:page:2}
```
