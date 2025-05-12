> ## SYOTAME – Gestion intelligente des zones de stationnement grâce à la vision par ordinateur

### 📂 Dossiers clés du projet

Les fichiers et dossiers suivants sont essentiels au bon fonctionnement du programme :

* `classes/StructureCLasses.py`
* `main/test.py`
* `images/` (images d'entrée et résultats illustrés)

### ❗ Problématiques identifiées

* 📌 Revoir la méthode de sauvegarde des observations dans le dossier `vues/`.
* ⚙️ Optimiser les fichiers :

  * `main/main.py`
  * `classes/reconnaissanceTexte.py`
  * Observation dans `search/`
* 🛠️ Améliorer la fonction `when_open(company)` (dans `classes/own_code/Structure.py`) pour fiabiliser l'extraction des horaires d'ouverture d’entreprise (actuellement des résultats erronés).
* 🅿️ Revoir `ParkingField()` dans `classes/own_code/ParkingPlace.py` pour une meilleure détection des places de stationnement, notamment celles délimitées par des bordures.
  👉 **Solution possible : intégrer YOLO pour une détection plus robuste.**

### 📝 Note de comptage

* **38** places libres détectées automatiquement sur l’image ci-dessous
* **5** sont réservées aux personnes en situation de handicap

![Illustration du parking](/images/park/park.jpg)

### 🧰 Librairies utilisées

```bash
pip install mysql-connector-python  # Connexion à la base de données MySQL
```

### 💡 Suggestions futures

* Intégrer **Apache Kafka** pour l’optimisation du traitement et de la transmission des données en temps réel.
