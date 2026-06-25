# Apache Kvrocks Distribution Packages via FPM

This repository builds **Linux distribution packages** for **Apache Kvrocks** using **GitHub Actions** and **FPM**.

It automates:
- fetching/building Apache Kvrocks from the official project,
- packaging the result into **`.deb`** files using **[FPM](https://fpm.readthedocs.io/en/latest/index.html)**,
- publishing the generated packages to the **GitHub Release**.

## Source project

Packages are built from:
- [apache/kvrocks](https://github.com/apache/kvrocks)

## What you get

For each release/tag, the workflow generates:
- **Debian/Ubuntu `.deb` packages** built on:
  - Ubuntu **22.04**, **24.04**, **26.04** for **x86_64**
  - Ubuntu **24.04** for **arm64**

## Notes

If you want to extend this project to support additional architectures or Ubuntu versions, the CI can be adapted to build multiple targets and upload all resulting artifacts to the **same GitHub Release**.

Pull requests are welcome—feel free to open one.