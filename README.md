# nitpreetb.github.io

A personal Quarto website created for DSCI 521 with blog posts in R and Python demonstrating data analysis workflows.

## Installation

This project requires the following software:

- **Quarto** version 1.10.18 or later
- **uv** version 0.12.10 or later
- **R** 4.6.1 or later

The Python environment is managed with `uv` and recorded in `uv.lock`. The R environment is managed with `renv` and recorded in `renv.lock`.

## Building the Site

Clone the repository and build from scratch:

```bash
git clone https://github.com/NitpreetB/nitpreetb.github.io.git
cd nitpreetb.github.io.git
```

Then install the Python dependencies at the top of the directory by running

```bash
uv sync
```

Then install R dependencies by running the following command in R

```r
renv::restore()
```

Render and preview the website using Quarto :

```bash
uv run quarto render
```

```bash
uv run quarto preview
```

running the preview command will allow you to view the webpage running on your local host

## Data Sources

The blog posts use the Palmer Penguins dataset, which is loaded from the `palmerpenguins` R and Python packages. 

