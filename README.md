# Housing-Price-Prediction

### Documentation pour le Repository de l'API

#### 📖 Description du Projet
Ce repository contient le code source de l'API de prédiction des prix des maisons utilisant FastAPI. Cette API prend en entrée diverses caractéristiques d'une maison et renvoie le prix prédit.

#### 🚀 Installation
Suivez les étapes ci-dessous pour installer et exécuter l'API en local.

1. **Cloner le Repository :**
   ```bash
   git clone https://github.com/abrahamkoloboe27/API-Housing-Price-Prediction.git
   cd API-Housing-Price-Prediction
   ```

2. **Créer et Activer un Environnement Virtuel :**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows, utilisez `venv\Scripts\activate`
   ```

3. **Installer les Dépendances :**
   ```bash
   pip install -r requirements.txt
   ```

4. **Lancer l'API :**
   ```bash
   uvicorn api:app --reload
   ```

#### 📝 Utilisation
Une fois l'API en cours d'exécution, vous pouvez envoyer des requêtes POST à l'endpoint `/predict` avec les caractéristiques de la maison pour obtenir une prédiction de prix.

#### 📄 Exemple de Requête avec `curl`
```bash
curl -X POST "http://127.0.0.1:8000/predict" -H "Content-Type: application/json" -d '{
    "area": 2640,
    "bedrooms": 2,
    "bathrooms": 1,
    "stories": 1,
    "mainroad": "no",
    "guestroom": "no",
    "basement": "no",
    "hotwaterheating": "no",
    "airconditioning": "no",
    "parking": 1,
    "prefarea": "no",
    "furnishingstatus": "furnished"
}'
```

#### 📄 Exemple de Requête avec JavaScript
```javascript
fetch("http://127.0.0.1:8000/predict", {
    method: "POST",
    headers: {
        "Content-Type": "application/json"
    },
    body: JSON.stringify({
        area: 2640,
        bedrooms: 2,
        bathrooms: 1,
        stories: 1,
        mainroad: "no",
        guestroom: "no",
        basement: "no",
        hotwaterheating: "no",
        airconditioning: "no",
        parking: 1,
        prefarea: "no",
        furnishingstatus: "furnished"
    })
})
.then(response => response.json())
.then(data => console.log(data));
```

#### 🔗 Liens Utiles
- [Documentation de FastAPI](https://fastapi.tiangolo.com/)
- [Repository GitHub](https://github.com/abrahamkoloboe27/API-Housing-Price-Prediction)




### Documentation pour le Repository de l'Application Streamlit

#### 📖 Description du Projet
Ce repository contient le code source de l'application Streamlit pour la prédiction des prix des maisons. Cette application fournit une interface utilisateur interactive pour entrer les caractéristiques d'une maison et obtenir une prédiction de prix.

#### 🚀 Installation
Suivez les étapes ci-dessous pour installer et exécuter l'application Streamlit en local.

1. **Cloner le Repository :**
   ```bash
   git clone https://github.com/abrahamkoloboe27/App-Streamlit-Housing-Price-Prediction.git
   cd App-Streamlit-Housing-Price-Prediction
   ```

2. **Créer et Activer un Environnement Virtuel :**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows, utilisez `venv\Scripts\activate`
   ```

3. **Installer les Dépendances :**
   ```bash
   pip install -r requirements.txt
   ```

4. **Lancer l'Application Streamlit :**
   ```bash
   streamlit run app.py
   ```

#### 📝 Utilisation
Une fois l'application Streamlit en cours d'exécution, ouvrez un navigateur et accédez à `http://localhost:8501` pour utiliser l'interface.

#### 📄 Exemple d'Utilisation
Entrez les caractéristiques de la maison dans l'interface et cliquez sur le bouton pour obtenir une prédiction de prix.

#### 🔗 Liens Utiles
- [Documentation de Streamlit](https://docs.streamlit.io/)
- [Repository GitHub](https://github.com/abrahamkoloboe27/App-Streamlit-Housing-Price-Prediction)

#### 📧 Contact
Pour toute question ou suggestion, veuillez contacter Abraham KOLOBOE à l'adresse email [abklb27@gmail.com](mailto:abklb27@gmail.com).

