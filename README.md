# 🦉 OLint

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.1-cyan?style=flat-square"/>
</p>

> **OLint** — Static Code Security Analyzer

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OLint is a static code security analyzer that scans source files for dangerous patterns, potential vulnerabilities, and bad practices. It uses the Python standard library only and writes JSON, CSV, and TXT results under a configurable output directory.

---

## ✨ Features

- Scan a single file (`--file`) or a folder (`--folder`) with optional recursive walk
- Severity filter via `--severity` (default INFO)
- Detects dangerous patterns, possible hardcoded secrets, and high-entropy string literals
- Exclude paths with repeatable `--exclude` globs
- Saves JSON, CSV, and TXT reports (each togglable) under `--output`
- Quiet and no-color modes for scripting and CI-friendly output

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OLint --file app.py
./OLint --folder ./src --severity WARNING --exclude '*/vendor/*'
./OLint --folder . --output olint_results --no-color
./OLint --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
