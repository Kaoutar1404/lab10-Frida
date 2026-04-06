# 🔐 Lab Frida — Analyse dynamique d'une application Android

> **Environnement :** Windows 10 · Python 3.13.11 · Frida 17.9.1 · Émulateur Android (Pixel 6 Pro API 37.0 — emulator-5554)  
> **Application cible :** Android Settings (`com.android.settings`)

---

## 📋 Table des matières

- [Étape 1 — Installation du client Frida](#étape-1--installation-du-client-frida)
- [Étape 2 — Installation ADB et connexion émulateur](#étape-2--installation-adb-et-connexion-émulateur)
- [Étape 3 — Déploiement de frida-server sur l'émulateur](#étape-3--déploiement-de-frida-server-sur-lémulateur)
- [Étape 4 — Test de connexion](#étape-4--test-de-connexion)
- [Étape 5 — Injection minimale](#étape-5--injection-minimale)
- [Étape 7 — Hooks réseau et système de fichiers](#étape-7--hooks-réseau-et-système-de-fichiers)
- [Résultats obtenus](#résultats-obtenus)

---

## Étape 1 — Installation du client Frida

### Commandes exécutées

```powershell
python --version
pip --version
pip install --upgrade frida frida-tools
frida --version
frida-ps --help
python -c "import frida, sys; print('frida', frida.__version__)"
