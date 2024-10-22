# FinML presentation latex source file repo

- to compile the tex file, make sure you have 'Metropolis' theme package installed.
- otherwise, you can change theme in `./scripts/cnbeamer.tex` file
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