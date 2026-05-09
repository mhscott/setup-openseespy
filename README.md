## v1.0.0 (Current)

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
