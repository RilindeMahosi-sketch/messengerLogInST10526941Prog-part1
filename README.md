# Mahosi Part 1

The submitted project is packaged as `mahosipoe part1.zip`. It is a NetBeans/Apache Ant Java project, so the ZIP itself is not directly executable.

## Requirements

- JDK (not only a JRE)
- Apache Ant
- `unzip` on Linux/macOS (Windows uses PowerShell)

## Run it

From the repository root on Linux/macOS:

```bash
chmod +x run.sh
./run.sh
```

On Windows, open Command Prompt in the repository root and run:

```bat
run.bat
```

You can also provide a different archive path:

```bash
./run.sh "/path/to/mahosipoe part1.zip"
```

The launcher extracts the archive to a temporary directory, finds its NetBeans `build.xml`, builds the project, and invokes its configured Ant `run` target. The temporary extracted files are removed when the launcher exits.

If Ant reports that no main class is configured, open the extracted project in NetBeans and set the project’s Main Class under **Project Properties → Run**, then recreate the ZIP.
