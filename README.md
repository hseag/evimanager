# eviManager

eviManager is the Windows service application for HSE AG's Colibri instruments.
It detects connected instruments, updates firmware, runs self-tests and exports
technical reports as PDF files. See the [User Guide](doc/doc/guide.md).

## Download

The precompiled Windows x64 portable EXE and its SHA-256 checksum are in
[`downloads/`](downloads/). The EXE includes the .NET runtime and requires no
installation. The application source code is not included in this repository.

## Documentation

The documentation can be rebuilt using only this repository and Python 3.11+:

```sh
python -m pip install -r doc/requirements-docs.txt
python -c "import shutil; shutil.copytree('downloads', 'doc/doc/downloads', dirs_exist_ok=True)"
python -m mkdocs build --strict -f doc/mkdocs.yml -d ../public
```

The generated site is in `public/` and includes the precompiled download. No .NET
SDK or access to the application repository is needed. A GitHub Pages workflow
can run these commands and publish that directory.

Releases are published to `main`; pre-release builds are published to
`pre-release`. Publication preserves `.github/` and `ci/`, so GitHub workflows
and their helper scripts can be maintained in this repository. New publication
branches inherit these directories from `main`. Other files are replaced by
the publication export.
