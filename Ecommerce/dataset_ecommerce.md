# 📊 Dataset E-Commerce - Guide Explicatif

## 🎯 Vue d'ensemble
Ce dataset contient des données de transactions e-commerce d'une entreprise de vente au détail en ligne, couvrant une période d'un an (décembre 2010 - décembre 2011).

## 📋 Structure du Dataset

### **Fichier**: `datasets/ecommerce.csv`
- **Taille**: 541,911 lignes de données
- **Période**: Décembre 2010 - Décembre 2011
- **Source**: Kaggle E-Commerce Sales Data
- **Encodage**: ISO-8859-1

### **Colonnes du Dataset**

| Colonne | Type | Description | Exemple |
|---------|------|-------------|---------|
| `InvoiceNo` | String | Numéro de facture unique | "536365" |
| `StockCode` | String | Code produit unique | "85123A" |
| `Description` | String | Nom/description du produit | "WHITE HANGING HEART T-LIGHT HOLDER" |
| `Quantity` | Integer | Quantité vendue | 6 |
| `InvoiceDate` | DateTime | Date et heure de la transaction | "12/1/2010 8:26" |
| `UnitPrice` | Float | Prix unitaire en livres sterling | 2.55 |
| `CustomerID` | Integer | Identifiant unique du client | 17850 |
| `Country` | String | Pays de la transaction | "United Kingdom" |

## 🌍 Couverture Géographique
- **Pays principaux**: Royaume-Uni, France, Allemagne, etc.
- **Portée**: International (ventes multi-pays)
- **Marché principal**: Europe

## 🛍️ Types de Produits
Le dataset contient principalement des articles de décoration et cadeaux :
- Articles de décoration (porte-clés, bougeoirs, etc.)
- Cadeaux et objets de collection
- Articles ménagers
- Jouets et jeux
- Accessoires de mode

## 📈 Métriques Clés Calculées
- **Revenus**: `Quantity × UnitPrice`
- **Année**: Extraction de l'année depuis `InvoiceDate`
- **Mois**: Extraction du mois depuis `InvoiceDate`
- **Mois de facturation**: Période mensuelle pour l'analyse

## 🔧 Nettoyage des Données
### **Étapes de préparation**:
1. **Suppression des annulations**: Exclusion des transactions avec quantité négative
2. **Filtrage des retours**: Exclusion des factures commençant par "C"
3. **Validation des prix**: Conversion en format numérique
4. **Calcul des revenus**: Multiplication quantité × prix unitaire
5. **Suppression des doublons**: Élimination des enregistrements dupliqués

## 📊 Analyses Possibles
### **Analyses de base**:
- Tendance des ventes mensuelles
- Top produits par revenus
- Répartition géographique des ventes
- Valeur moyenne des commandes (AOV)

### **Analyses avancées**:
- Segmentation RFM (Récence, Fréquence, Monétaire)
- Analyse des clients VIP
- Identification des opportunités de cross-selling
- Analyse saisonnière des ventes

## 🎯 Objectifs Business
- **Optimisation des stocks**: Identifier les produits les plus vendus
- **Fidélisation client**: Analyser le comportement d'achat
- **Expansion géographique**: Cibler les marchés les plus rentables
- **Amélioration des revenus**: Stratégies d'upselling et cross-selling

## ⚠️ Points d'Attention
- **Données manquantes**: Certains `CustomerID` peuvent être nuls
- **Période limitée**: Seulement 1 an de données
- **Devise**: Tous les prix sont en livres sterling
- **Retours**: Les annulations sont identifiables par le préfixe "C"

## 🚀 Utilisation Recommandée
Ce dataset est idéal pour :
- L'apprentissage de l'analyse de données e-commerce
- Les projets de data science sur le retail
- L'analyse de comportement client
- Les études de cas business intelligence

---
*Dataset préparé pour l'analyse des ventes e-commerce - Portfolio Data Analysis*
