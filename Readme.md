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
