# FinML presentation latex source file repo

## compilation config

- to compile the tex file, make sure you have 'Metropolis' theme package and 'STIX Two Math' font package installed.
- otherwise, you can change theme and font in `./scripts/cnbeamer.tex` file (some common configs I use when creating a beamer)
- if you use vscode and latex-workshop, I suggest use `latexmk` for automatic compilation, my compilation config is something like (%***% is vscode's placeholder, you can define it in the vscode config)

```json
{
    "name": "latexmk",
    "command": "latexmk",
    "args": [
        "-synctex=1",
        "-interaction=nonstopmode",
        "-file-line-error",
        "-output-format=pdf",
        "-auxdir=%WORKSPACE_FOLDER%/temp",
        "-outdir=%OUTDIR%",
        "-xelatex",
        "%DOC%"
    ]
}
```

## To Be Done

- [ ] may need to add a explanation of SDF between page 7 and 8 of the slides