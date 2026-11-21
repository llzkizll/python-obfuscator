<h1 align="center">
  <img src="./assets/python-obfuscator.gif" width="900" alt="Python Obfuscator by ZKIZ">
</h1>

<p align="center">A command-line tool that turns a Python script into a harder-to-read copy.</p>

<p align="center">
  <a href="https://github.com/llzkizll"><img src="./assets/github.png" height="34" alt="ZKIZ on GitHub"></a>
</p>

## Quick start

From the repository folder, install the dependencies and open the menu.

```powershell
python -m pip install -r requirements.txt
python "ZKIZ OBFUSCATOR.py"
```

Choose a mode and enter the path to a `.py` file. The tool writes its Python output next to the input file.

| Menu option | Output |
| --- | --- |
| **1 · Protect Python** | A single-line wrapper named `protected_<filename>.py`. |
| **2 · Protect + EXE** | A Python wrapper and a Windows executable in `dist/`. Run this option on Windows. |
| **3 · Obfuscate only** | A layered wrapper named `obf_<filename>.py`. |

## Compatibility

Run the generated Python files with the same Python major and minor version used to create them. The wrappers contain version-specific Python bytecode. [Python documentation](https://docs.python.org/3/library/marshal.html)

Executable builds use PyInstaller. [PyInstaller documentation](https://pyinstaller.org/en/stable/)
