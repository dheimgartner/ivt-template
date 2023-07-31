# ivt-template

Make sure to set `-shell-escape` flag!

If you are using `LaTeX workshop` add the following to your (workspace) `settings.json`

```
{
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-shell-escape",
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOC%"
            ]
        }
    ],
}
```