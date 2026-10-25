# 🦉 OHeaders

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OHeaders** — Security Headers Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OHeaders — Security Headers Auditor. It provides single URL audit with full redirect-chain capture (stdlib urllib, custom UA, timeout, TLS verify toggle). Findings and exports support authorised defensive assessments within the OwlSec Toolkit.

---

## ✨ Features

- Single URL audit with full redirect-chain capture (stdlib urllib, custom UA, timeout, TLS verify toggle)
- Deep CSP analyzer — directive parser, fallback resolution, nonce/hash/strict-dynamic awareness, meta-tag CSP discovery, report-only detection, score
- HSTS analyzer — max-age tiers, includeSubDomains, preload-list eligibility check
- Cookie auditor — Secure / HttpOnly / SameSite, __Host- / __Secure- prefix rules, scope, lifetime
- CORS checker — active Origin probes (evil / null), reflected origin, wildcard + credentials detection
- Clickjacking — X-Frame-Options vs frame-ancestors

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OHeaders                                     # interactive menu
./OHeaders --json -o report.json
./OHeaders --url https://example.com
./OHeaders --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
