## v1.0.2 (Current)

### Changes from v1.0.1
- Optional specification of openseespy version (default: "latest")

### Example Usage

```yml
- name: Setup OpenSeesPy
  uses: mhscott/setup-openseespy@v1
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
  uses: mhscott/setup-openseespy@v1
  with:
    opsvis: true
```

## v1.0.0

Minimal GitHub Action for installing OpenSeesPy via pip.

### Features
- Initial release
- Installs OpenSeesPy in GitHub Actions workflows
- Assumes Python is already configured in the workflow
- Supports Ubuntu, Windows, and macOS runners

### Example Usage

```yml
- name: Setup OpenSeesPy
  uses: mhscott/setup-openseespy@v1
```

---

## v2.0.0 (Planned)

Build OpenSeesPy from source using CMake.

### Planned Features
- Optional MPI support
- Optional HDF5 support
- Optional custom OpenSees branch or commit checkout
- Cross-platform support for Ubuntu, Windows, and macOS runners
