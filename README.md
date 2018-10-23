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

### Indsæt et billede

```latex
\begin{figure}[h]
    \centering
    \includegraphics[scale=1]{sti/til/figur/figurFilNavn.png}
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
