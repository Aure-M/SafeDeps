# 🛡️ SafeDeps: Python Dependency Vulnerability Scanner

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🇫🇷 Français

### À propos
**SafeDeps** est un outil de sécurité léger conçu pour scanner récursivement vos projets à la recherche de fichiers `requirements.txt`. Il identifie les vulnérabilités connues dans vos dépendances Python en interrogeant l'API **Google OSV (Open Source Vulnerabilities)**.

### Caractéristiques principales
* **Recherche Récursive** : Localise automatiquement tous les fichiers `requirements.txt` dans les sous-dossiers.
* **Analyse Intelligente** : Supporte les opérateurs de version `==`, `>=` et `~=`.
* **Filtrage Précis** : Analyse les rapports de vulnérabilité pour ne retenir que ceux impactant vos contraintes spécifiques.
* **Intégration CI/CD** : Le script retourne un code de sortie `1` en cas de vulnérabilités **HIGH** ou **CRITICAL**, idéal pour bloquer des pipelines de déploiement non sécurisés.

### Installation
```bash
git clone [https://github.com/Aure-M/SafeDeps](https://github.com/Aure-M/SafeDeps/)
cd SafeDeps
pip install requests pandas
python vulnerability_scanner.py
```

# 🛡️ SafeDeps: Python Dependency Vulnerability Scanner

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Security: OSV.dev](https://img.shields.io/badge/Security-OSV.dev-orange.svg)](https://osv.dev/)

## 📝 Description
**SafeDeps** is a specialized security utility designed to safeguard your software supply chain. It recursively audits your project directories to locate `requirements.txt` files and cross-references your dependencies against the **Google OSV (Open Source Vulnerabilities)** database.

Unlike basic scanners, SafeDeps understands Python versioning logic, ensuring that vulnerability reports are contextually relevant to your specific version constraints.

## ✨ Key Features
* **Recursive Discovery**: Automatically traverses your project tree to find all dependency files.
* **Version-Aware Analysis**: Intelligent parsing of `==` (fixed), `>=` (minimum), and `~=` (compatible) operators.
* **Smart Filtering**: Dynamically filters API results to pinpoint vulnerabilities that specifically impact your environment.
* **DevOps Integration**: Designed for CI/CD pipelines with automated exit codes (Exit 1 on Critical/High risks).
* **Data-Driven**: Leverages `pandas` for structured analysis and clear reporting.



## 🚀 Getting Started

### Prerequisites
* Python 3.8 or higher
* `requests` and `pandas` libraries

### Installation
```bash
git clone [https://github.com/Aure-M/SafeDeps](https://github.com/Aure-M/SafeDeps/)
cd SafeDeps
pip install requests pandas
python vulnerability_scanner.py
```
