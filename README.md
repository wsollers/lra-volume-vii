# lra-volume-vii

**Volume VII: Advanced Logic** — Overleaf-ready standalone repository.

## Structure

```text
volume-vii.tex          — full-volume root (Overleaf main document)
volume-vii-<book>.tex   — individual book roots
common/               — shared LaTeX infrastructure supplied by lra-common; ignored here
bibliography/         — per-book bibliography shards
volume-vii/             — all LaTeX content for this volume
```

## Overleaf

Upload or checkout `common/` beside this repository's TeX roots, then set the main document to `volume-vii.tex` for the full volume or to one of the book roots:

```text
volume-vii-category-theory.tex, volume-vii-lambda-calculus.tex, volume-vii-model-theory.tex, volume-vii-proof-theory.tex, volume-vii-type-theory.tex
```

`common/` is ignored by git in this volume repo; edit shared infrastructure in `lra-common`.

## Building locally

```powershell
python F:\repos\lra-governance\tools\governance\build_volume_docker.py --root F:\repos\lra-volume-vii --common-root F:\repos\lra-common
```
