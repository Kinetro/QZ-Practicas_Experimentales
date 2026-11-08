# FORM-FB-01: Fichas bibliográficas

Universidad Técnica Estatal de Quevedo (UTEQ) · Carrera de Software

Aplicaciones Distribuidas · 7mo nivel · Paralelo B

Docente: Ing. Gleiston Cicerón Guerrero Ulloa

Estudiante: Zambrano Yong Angel Daniel

Semana 2 · 08/11/2026

## Archivos de esta carpeta

| Archivo | Descripción |
|---|---|
| `fichas.tex` | Documento principal en LaTeX con las 5 fichas bibliográficas |
| `referencias.bib` | Referencias para biblatex (estilo IEEE) |
| `logo-uteq.jpg` | Logo de la universidad para la carátula |
| `fichas.pdf` | Documento compilado |

## Fuentes

| Ficha | Fuente | DOI |
|---|---|---|
| 1 | Ferreira et al., IEEE Access, 2025 | [10.1109/ACCESS.2025.3558923](https://doi.org/10.1109/ACCESS.2025.3558923) |
| 2 | Ferreira et al., Journal of Cloud Computing, 2024 | [10.1186/s13677-024-00716-7](https://doi.org/10.1186/s13677-024-00716-7) |
| 3 | Ahmed et al., Radioelectronic and Computer Systems, 2023 | [10.32620/reks.2023.2.14](https://doi.org/10.32620/reks.2023.2.14) |
| 4 | Zhang et al., ACM Computing Surveys, 2024 | [10.1145/3636553](https://doi.org/10.1145/3636553) |
| 5 | Gorbenko et al., Radioelectronic and Computer Systems, 2021 | [10.32620/reks.2021.4.13](https://doi.org/10.32620/reks.2021.4.13) |

## Cómo compilar

Compilador: `pdflatex` con `biber` para la bibliografía.

Archivo principal: `fichas.tex`

Orden de comandos, desde esta carpeta:

```bash
pdflatex fichas.tex
biber fichas
pdflatex fichas.tex
pdflatex fichas.tex
```

O en un solo paso:

```bash
latexmk -pdf fichas.tex
```

Dependencias:

- TeX Live 2022 o superior, o MiKTeX en Windows.
- `biber`.
- Paquetes: `biblatex`, `biblatex-ieee`, `babel` (`spanish` y `american`), `csquotes`, `geometry`, `graphicx`, `xcolor`, `enumitem`, `hyperref`, `lmodern`.

En Overleaf: subir los cuatro archivos y en Menu → Settings elegir Compiler: pdfLaTeX. Overleaf corre `biber` solo.
