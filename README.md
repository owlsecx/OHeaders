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

HTTP security headers auditor & hardening advisor

---

## ✨ Features

- Single URL audit with full redirect-chain capture (stdlib urllib, custom UA, timeout, TLS verify toggle)
- Deep CSP analyzer — directive parser, fallback resolution, nonce/hash/strict-dynamic awareness, meta-tag CSP discovery, report-only detection, score
- HSTS analyzer — max-age tiers, includeSubDomains, preload-list eligibility check
- Cookie auditor — Secure / HttpOnly / SameSite, __Host- / __Secure- prefix rules, scope, lifetime
- CORS checker — active Origin probes (evil / null), reflected origin, wildcard + credentials detection
- Clickjacking — X-Frame-Options vs frame-ancestors
- XCTO, Referrer-Policy, Permissions-Policy, COOP, COEP, CORP, Cache-Control, info-disclosure checks
- HTTP→HTTPS upgrade check + TLS certificate reader (issuer, subject, SAN match, expiry, protocol, cipher)
- Weighted A+…F grade with per-category subscores
- Remediation generator — recommended CSP, Nginx, Apache, Caddy, IIS and HAProxy config snippets
- Batch mode (threaded) with summary table
- Baseline snapshots (JSON) + regression diff
- Offline raw-header analysis (paste or file)
- Save report (TXT / CSV / JSON) with location chooser

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OHeaders
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
