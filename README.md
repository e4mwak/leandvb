# Analog Radio Hunter DATV LeanDVB Package

This repository contains the external `leandvb.exe` backend source package used by Analog Radio Hunter DATV RX.

## Purpose

- Keep the DATV backend separate from the main app EXE.
- Publish the matching modified LeanDVB source and license materials in this repository and its releases.
- Let users download `leandvb.exe` manually and place it in `DATV\leandvb.exe` next to the main app.

## Upstream origin

- Upstream project: `https://github.com/pabr/leansdr`
- LeanDVB project page: `http://www.pabr.org/radio/leandvb`

## What to publish

- `source/` directory from the repository root
- `LICENSE.txt`
- `BUILD_WINDOWS.md`
- `UPSTREAM.md`
- `MODIFIED_FILES.md`
- your built `leandvb.exe` binary as a release asset

## Repository

- Repository URL: `https://github.com/e4mwak/leandvb`
- Recommended download point for users: the repository `Releases` page

## User install workflow

1. Download your `leandvb.exe`.
2. Put it in the main app folder under `DATV\leandvb.exe`.
3. In Analog Radio Hunter, leave the DATV Backend field empty or browse to that file manually.

## Notes

- This package is intended for the external DATV backend workflow.
- The main app launches `leandvb.exe` as a separate process.
