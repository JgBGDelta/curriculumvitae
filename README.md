<p align="center">
  <a href="https://builtwithnix.org"><img src="https://builtwithnix.org/badge.svg" alt="Built with nix badge"></a>
  <a href="https://github.com/JgBGDelta/curriculumvitae/commits/main"><img alt="github last commit" src="https://img.shields.io/github/last-commit/JgBGDelta/curriculumvitae?color=98c379&style=for-the-badge"></a>
</p>

> **_curriculum vitae_ (cur·ric·u·lum vi·tae)**
>
> A short account of one's career and qualifications prepared typically by an applicant for a position.

# Curriculum Vitae

English CV of **Jorge Barroso García**, software developer and Computer Science and Business Management student at the University of Alcalá.

The document uses the [moderncv](https://github.com/moderncv/moderncv) banking style. The source is [`cv.tex`](cv.tex). A version tag publishes `cv.pdf` with GitHub Actions; the latest release is [here](https://github.com/JgBGDelta/curriculumvitae/releases/latest/download/cv.pdf).

## Building

This repository builds with [Nix](https://nixos.org):

```sh
# Reproducible build. Output: result/cv.pdf
nix build github:JgBGDelta/curriculumvitae
```

For local iteration, enter the development shell and use [just](https://github.com/casey/just):

```sh
nix develop
just build                          # writes ./cv.pdf
just install /path/to/destination   # copies cv.pdf there
```
