#Code syntax highlight
Indsæt dette i din preamble for syntax highlight
```LaTeX
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% code
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Adds code snippet functionality
\usepackage{listings}						% Placer kildekode i dokumentet med \begin{lstlisting}...\end{lstlisting}
\renewcommand{\lstlistingname}{Kodeudrag}   % Listing -> Kodeudrag
\usepackage{tcolorbox}

\definecolor{commentGreen}{RGB}{34,139,24}
\definecolor{stringPurple}{RGB}{208,76,239}
\definecolor{keywordPurple}{RGB}{168,26,143}
\definecolor{indentifierPurple}{RGB}{91,44,151}
\definecolor{stringRed}{RGB}{194,29,32}
\definecolor{commentGreen}{RGB}{22,150,25}
\usepackage{tgheros}

\lstset{language=C,
  caption={Uddrag af C program},
  label=DescriptiveLabel,
  numbers=left, numberstyle=\tiny,
  backgroundcolor=\color{black!1},
}

\lstdefinestyle{customc}{
  belowcaptionskip=1\baselineskip,
  breaklines=true,
  frame=tlrb,
  rulecolor=\color{black!20},
  xleftmargin=\parindent,
  language=C,
  showstringspaces=false,
  basicstyle=\footnotesize\ttfamily,
  keywordstyle=\bfseries\color{keywordPurple},
  commentstyle=\itshape\color{commentGreen},
  identifierstyle=\color{indentifierPurple},
  stringstyle=\color{stringRed},
}

\lstdefinestyle{customasm}{
  belowcaptionskip=1\baselineskip,
  frame=L,
  xleftmargin=\parindent,
  language=[x86masm]Assembler,
  basicstyle=\footnotesize\ttfamily,
}

\lstset{escapechar=@,style=customc}

%%syntax highlight simple
\definecolor{hisyntxcolor}{rgb}{0.95, 0.95, 0.96}

\newtcbox{\hisyntx}{nobeforeafter, colback=hisyntxcolor!80,boxrule=0pt,boxsep=0pt,left=4pt,right=4pt,top=3.5pt,bottom=3.5pt,tcbox raise base}
```
