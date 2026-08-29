# Tabla Periódica e Ingeniería de Materiales

## Run the app

Run as a desktop app:

```bash
../.venv/bin/flet run
```

Run as a web app:

```bash
../.venv/bin/flet run --web
```

## Dependencies

Dependencies are declared in `pyproject.toml`.

Main runtime dependency:

- `flet>=0.86.5`

Development dependencies:

- `flet-cli>=0.86.5`
- `flet-desktop>=0.86.5`
- `flet-web>=0.86.5`
- `flet[test]>=0.86.5`

## Verify

```bash
../.venv/bin/python -m py_compile src/main.py src/algorithm.py
../.venv/bin/flet --version
```

Flet integration tests can be run with:

```bash
../.venv/bin/flet test macos .
```

That command may provision Flutter SDK 3.44.8 on first run.

## App Files

- `src/main.py`: main Flet UI
- `src/algorithm.py`: electronic configuration and valence calculations
- `src/elements.json`: element data
- `src/table.json`: periodic table layout
- `src/colors.json`: category colors

## Build the app

### Android

```bash
flet build apk -v
```

For more details on building and signing `.apk` or `.aab`, refer to the [Android Packaging Guide](https://flet.dev/docs/publish/android/).

### iOS

```bash
flet build ipa -v
```

For more details on building and signing `.ipa`, refer to the [iOS Packaging Guide](https://flet.dev/docs/publish/ios/).

### macOS

```bash
flet build macos -v
```

For more details on building macOS package, refer to the [macOS Packaging Guide](https://flet.dev/docs/publish/macos/).

### Linux

```bash
flet build linux -v
```

For more details on building Linux package, refer to the [Linux Packaging Guide](https://flet.dev/docs/publish/linux/).

### Windows

```bash
flet build windows -v
```

For more details on building Windows package, refer to the [Windows Packaging Guide](https://flet.dev/docs/publish/windows/).

### Web

```bash
flet build web -v
```

For more details on building Web app, refer to the [Web Packaging Guide](https://flet.dev/docs/publish/web/).
