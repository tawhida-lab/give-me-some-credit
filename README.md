# Credit Risk Prediction 💳

## Contexte
Prédiction de la probabilité de défaut de paiement financier
150 000 clients · 11 variables · 4 features créées · Kaggle Competition

---

## Stack technique
Python · XGBoost · SHAP · scikit-learn · Pandas · Matplotlib · Seaborn

---

## Résultats

| Métrique | Valeur |
|---|---|
| AUC-ROC | 0.85 |
| Recall Défaut | 71% |
| Accuracy | 83% |

---

## Structure du projet

- Phase 1 : EDA & Nettoyage (12 → 11 colonnes, anomalies corrigées)
- Phase 2 : Feature Engineering (4 nouvelles variables créées)
- Phase 3 : Modélisation XGBoost (scale_pos_weight = 13.96)
- Phase 4 : Interprétabilité SHAP

---

## Top 6 drivers du défaut (SHAP)

1. `total_retards` (somme retards de paiement — créé) ✅
2. `ratio_utilisation_age` (utilisation crédit / âge — créé) ✅
3. `score_risque` (score composite global — créé) ✅
4. `RevolvingUtilizationOfUnsecuredLines`
5. `ratio_dette_revenu` (dette / revenu — créé) ✅
6. `age`

> 4 des 6 variables les plus importantes ont été créées par Feature Engineering

---

## Fichiers du repo
give-me-some-credit/
├── give-me-some-credit.ipynb
└── README.md
---

## Comment reproduire

1. Accepter les règles sur kaggle.com/c/give-me-some-credit
2. Ouvrir le notebook Kaggle
3. Run All

---

## Dataset
[Give Me Some Credit — Kaggle](https://www.kaggle.com/c/GiveMeSomeCredit)
