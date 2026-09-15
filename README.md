# TP 01 - HTTP : Le jeu de piste
**Mission 0 : Découverte des outils (Postman, Bruno, Insomnia)**

**Nom :** Emma-Gabrielle FOUGEROUX
**Classe :** BTS SIO SLAM 2

---

## 1. Outils utilisés
Pour ce TP, j'ai installé et testé trois clients HTTP :
* **Postman** (nécessite un compte, connecté avec GitHub)
* **Bruno** (très simple et léger)
* **Insomnia** (interface claire)

---

## 2. Requête GET simple

* **URL :** `https://jsonplaceholder.typicode.com/posts`
* **Méthode :** `GET`
* **Objectif :** Récupérer la liste des articles.
* **Code retour :** `200 OK` (la requête a fonctionné).
* **Réponse :** On reçoit un tableau de données au format JSON avec les posts.

### Captures d'écran GET :
* **Postman :**  
  ![GET Postman](screenshots/postman_get.png)
* **Bruno :**  
  ![GET Bruno](screenshots/bruno_get.png)
* **Insomnia :**  
  ![GET Insomnia](screenshots/insomnia_get.png)

---

## 3. Requête POST avec données

* **URL :** `https://jsonplaceholder.typicode.com/posts`
* **Méthode :** `POST`
* **Header ajouté :** `Content-Type: application/json`
* **Corps envoyé (Body en JSON) :**
```json
{
  "title": "Mon premier post",
  "body": "Créé avec [Postman/Bruno/Insomnia]",
  "userId": 1
}
