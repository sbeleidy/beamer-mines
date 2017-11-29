# beamer-mines

Beamer theme for the Colorado School of Mines.

**This is NOT an official Mines theme but is only an attempt at an implementation.**


## How to use

Clone or copy the `beamercolorthememines.sty` file into your TeX directory or project then in your beamer project use:

```LaTeX
\usecolortheme{mines}
```

<!-- TODO: Move this to environment/command taking image, title, author and subtitle as params -->
## First Slide

The following code can be used to make a nicer title slide:

```LaTeX
{
        \usebackgroundtemplate{\scalebox{-1}[1]{\includegraphics[width=\paperwidth, height=\paperheight]{PATH/TO/BACKGROUND/IMAGE/FILE.png}}}
        \begin{frame}[plain]
            \color{white}
            \vspace{4.8cm}
            {\Huge \fontspec{Montserrat Bold} PRESENTATION TITLE} \\
            \vspace{-0.2cm}
            {\color{white} \rule{\linewidth}{0.1mm}}
            \color{mineslightblue}
            {\Large \fontspec{Montserrat Light} SUBTITLE}
            \begin{spacing}{1.3}
            {\Large \fontspec{Montserrat Light} by} {\Large \fontspec{Montserrat Regular} AUTHOR NAME}
            \end{spacing}
        \end{frame}
    }
```

## What you need

Make sure you have LaTeX installed.

Make sure you install the [Montserrat fonts](https://fonts.google.com/specimen/Montserrat).

You'll need to use `xelatex` not `pdflatex` for compilation due to the use of the fontspec package. The settings.json file in this repo can be used with [VS Code](https://code.visualstudio.com/) and the [LaTeX workshop plugin](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) for the workspace or user settings.

