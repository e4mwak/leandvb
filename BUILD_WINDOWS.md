# Build LeanDVB on Windows

These are the commands used in this project to build the modified `leandvb.exe`.

## Build environment

- Windows
- Radioconda / MinGW toolchain

## Example build command

```bat
set PATH=C:\radioconda\Library\mingw-w64\bin;%PATH%
cd apps
mingw32-make.exe leandvb VERSION=arh-external LDFLAGS=-lws2_32
```

## Output

- Expected output binary: `apps\leandvb.exe`

## Release step

Copy the built binary into your release package as:

```text
leandvb.exe
```

Users should place that file next to the main app inside:

```text
DATV\leandvb.exe
```

Recommended distribution model:

- Keep source code, license text, and build notes in `https://github.com/e4mwak/leandvb`
- Upload `leandvb.exe` as a GitHub Release asset
