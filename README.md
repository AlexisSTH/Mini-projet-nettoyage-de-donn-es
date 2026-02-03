# 🧹 Nettoyage de Données

## 📋 Description

Projet de nettoyage d'un dataset clients contenant 30 lignes avec diverses anomalies (doublons, valeurs manquantes, formats incohérents, outliers).

## 🔍 Problèmes → Solutions

| Problème | Solution |
|----------|----------|
| Doublons | `drop_duplicates()` |
| Valeurs manquantes | Médiane / Mode |
| Formats dates | `pd.to_datetime()` |
| Textes incohérents | `.str.lower().str.strip()` |
| Ages aberrants | Remplacés par médiane |
| Montants négatifs | `.abs()` |
| Montants excessifs | Cappés à 10,000€ |

## 📈 Résultats

AVANT                    APRÈS
─────────────────────────────────────
30 lignes               28 lignes
15+ valeurs manquantes  0 manquantes
3 formats dates         1 format
Ages: -5 à 150          Ages: 18 à 100
Montants: -500 à 50000  Montants: 0 à 10000

