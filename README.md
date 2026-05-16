Minimal GitHub Action for installing OpenSeesPy via pip.

## Features
- Installs OpenSeesPy in GitHub Actions workflows
- Supports Ubuntu, Windows, and macOS runners
- Assumes Python is already configured in the workflow
  - Does _not_ attempt to resolve dependencies between Python, OpenSeesPy, and the runner's operating system
  - Python 3.12 and OpenSeesPy >= 3.5.1.2 are recommended

## v1.0.3 (Current)

### Changes from v1.0.2
- Force installs `openseespylinux`, `openseespywin`, and `openseespymac` because the `openseespy` wrapper is not bound to specific operating system versions
- Prints Python and OpenSeesPy version information

### Example Usage

```yml
- name: Setup OpenSeesPy
  uses: mhscott/setup-openseespy@v1
  with:
    version: "3.7.1.2"
    opsvis: true
```

## v1.0.2

### Changes from v1.0.1
- Optional specification of openseespy version (default: "latest")

### Example Usage

```yml
- name: Setup OpenSeesPy
  uses: mhscott/setup-openseespy@v1.0.2
  with:
    version: "3.7.1.2"
    opsvis: true
```

## v1.0.1

### Changes from v1.0.0
- Optional install of [opsvis](https://github.com/sewkokot/opsvis) (default: false)

### Example Usage

```yml
- name: Setup OpenSeesPy
  uses: mhscott/setup-openseespy@v1.0.1
  with:
    opsvis: true
```

## v1.0.0

### Initial Release

### Example Usage

```yml
- name: Setup OpenSeesPy
  uses: mhscott/setup-openseespy@v1.0.0
```

---

## v2.0.0 (Planned)

Build OpenSeesPy from source using CMake.

### Planned Features
- Optional MPI support
- Optional HDF5 support
- Optional custom OpenSees branch or commit checkout
- Cross-platform support for Ubuntu, Windows, and macOS runners
