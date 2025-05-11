# 🧭 Dashboard Streamlit – Visualisation des prédictions

Ce dossier contient un tableau de bord interactif développé avec **Streamlit**.  
Il permet de visualiser et d’explorer les résultats de classification automatique sur plus de **150 000 avis produits**.

---

## 🔍 Objectif

Ce dashboard a été conçu pour :

- Observer la **répartition des prédictions** sur plusieurs années
- Explorer **l'évolution dans le temps de chaque typologie de problème**
- Sélectionner un **produit parmi les plus commentés**, selon chaque **tranche de note**
   - ➤ Cela permet de **détecter à grande échelle les produits problématiques**, selon leur niveau de satisfaction
   - ➤ D'avoir accés aux types de commentaires concernés
- Explorer des exemples concrets de **commentaires annotés automatiquement**
- **Télécharger des fractions du dataset** au format Excel ou CSV pour analyse hors ligne

---

## 🗄 Source des données

À l’origine, l’application interrogeait une base de données **hébergée par Supabase**.  
Cependant, pour éviter les interruptions dues aux quotas ou à l’indisponibilité du service, la version actuelle est **branchée sur un fichier `.parquet` local** (`data/reviews_full.parquet`) qui **simule la base Supabase**.

⚠️ Ce dépôt contient l’ensemble des données prédites afin d’alimenter un dashboard Streamlit. Il est utilisé à des fins de démonstration uniquement.
    
---

## 🚀 Lancer le dashboard

Depuis le dossier `Amazon_dashboard_streamlit`, lancez l'application avec la commande :

```bash
streamlit run Page_accueil.py