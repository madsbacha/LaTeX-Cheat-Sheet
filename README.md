# LaTeX Cheat Sheet

# Indholdsfortegnelse

 * [Indsæt et billede](#indsæt-et-billede)
 * Tekst formatering
   * [Italic](#italic)
   * [Bold](#bold)
 * [Citering](#citering)
 * [Referering til label](#referering-til-label)
 * [Lav et label](#lav-et-label)
 * [Kommentar](#kommentar)
 * Macros
   * [Citation needed](#citation-needed)
 * [Centrering](#centrering)

### Indsæt et billede

```latex
\begin{figure}[h]
    \centering
    \includegraphics[scale=1]{sti/til/figur/figurFilNavn.png}
%   \includegraphics[width=\textwidth]{sti/til/figur/figurFilNavn.png} % Match width til sidens bredde
    \caption{Figur tekst \cite{Citelabel}}
    \label{label}
\end{figure}
```

### Italic

```latex
\textit{Det her er italic}
```

### Bold

```latex
\textbf{Det her er bold}
```

### Citering

```latex
\cite{Kildelabel}
```

### Referering til label

```latex
\ref{label}
```

### Lav et label

```latex
\label{type:labelnavn}
```

### Kommentar

```latex
% Dette er en kommentar
```

### Citation needed

```latex
LaTeX er awesome!\citationneeded
```

For at kunne bruge `\citationneeded`, skal følgende tilføjes til dit LaTeX dokument.
```latex
%Citation needed command
\newcommand{\citationneeded}[1][]{\color{blue} [Citation needed]\color{black}}
```

### Centrering
```latex
\begin{center}
    Centreret tekst
\end{center}
```
