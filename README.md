# TP1 — Intégration des données avec SSIS


Extraction de données depuis un fichier plat vers une base de données **SQL Server 2022** via un package **SSIS**.  
Réalisé dans le cadre du cours Business Intelligence — Université USMBA.

---

## 🛠️ Outils

- SQL Server 2022 + SSMS
- Visual Studio 2022 + Extension SSIS
- Langage de script : C#

---

## 📦 Contenu du package

Le package SSIS exécute 3 tâches dans l'ordre :

1. **Script C#** — affiche un message de démarrage
2. **Tâche SQL** — vide la table (`TRUNCATE TABLE`)
3. **Data Flow** — lit le fichier `.txt` et charge les données dans SQL Server

---

## 🚀 Exécution

1. Ouvrir le projet dans **Visual Studio 2022**
2. Adapter le chemin du fichier `clients.txt` dans le Connection Manager
3. Vérifier la connexion OLE DB vers `BD_TP1_SSIS`
4. Lancer avec `F5` ou `Déboguer → Démarrer le débogage`
5. Vérifier dans SSMS : `SELECT * FROM dbo.TP1_ETL_Client` → **11 lignes**

---

## 👤 Auteur

**Mouhamed NAZIROU. NDIAYE.** — USMBA21033 — 2025/2026
**ETUDIANT EN MACHINE LEARNING ET INTELLIGENCE MULTIMEDIA**