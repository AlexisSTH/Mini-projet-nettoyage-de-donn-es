# 🧹 Nettoyage de Données

## 📋 Description

Projet de nettoyage d'un dataset clients contenant 30 lignes avec diverses anomalies (doublons, valeurs manquantes, formats incohérents, outliers).


## ✅ Solutions Appliquées

| Problème | Solution |
|----------|----------|
| Doublons | `drop_duplicates()` |
| NaN numériques | Médiane |
| NaN catégoriels | Mode ou "Inconnu" |
| Dates | `pd.to_datetime()` |
| Textes | `.str.lower().str.strip()` |
| Ages < 18 | Remplacés par médiane |
| Ages > 100 | Remplacés par médiane |
| Montants négatifs | `.abs()` |
| Montants excessifs | Cappés à 10,000€ |

## 🛠️ Technologies

- Python 3.8+
- Pandas
- NumPy

