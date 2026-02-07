# 📊 ETF & Portfolio Comparator

Un outil professionnel pour analyser et comparer des ETFs ainsi que des portefeuilles complexes avec rééquilibrage automatique.

## 🚀 Fonctionnalités Clés

- **Comparaison Multi-Devises** : Passage dynamique entre EUR, USD et GBP avec taux de change historiques.
- **Support Total Return** : Calculs basés sur les prix ajustés (incluant le réinvestissement des dividendes).
- **Constructeur de Portefeuilles** : Créez vos propres paniers d'ETFs avec des poids personnalisés.
- **Rééquilibrage Automatique** : Simulez des stratégies de rééquilibrage (Mensuel, Trimestriel, Annuel, etc.).
- **Analyse de Risque** : Calcul de la Volatilité, de la Tracking Error et de la Tracking Difference.
- **Visualisation des Actifs** : Répartition sectorielle et géographique (via les métadonnées Yahoo Finance).

## 🛠 Installation

1. **Cloner le dépôt** :
   ```bash
   git clone <url-du-repo>
   cd etf_comparator
   ```

2. **Installer les dépendances** :
   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows: venv\Scripts\activate
   pip install yfinance pandas numpy
   ```

3. **Récupérer les données** :
   ```bash
   python get_data.py
   ```

4. **Lancer l'application** :
   Ouvrez simplement `page.html` dans votre navigateur.

## 📁 Structure du Projet

- `get_data.py` : Script Python pour télécharger les prix, le FX et les métadonnées.
- `page.html` : L'application web interactive (Single Page App).
- `data.json` : Base de données locale générée par le script.

## 📝 Configuration

Pour ajouter de nouveaux ETFs, modifiez le dictionnaire `tickers_config` dans le fichier `get_data.py` et relancez le script.

---
*Note : Les données sont fournies par l'API Yahoo Finance à titre informatif.*
