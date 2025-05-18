# Web Infrastructure Design — 3. Scale Up

## README

### Description
Ce projet consiste à concevoir une infrastructure web évolutive en séparant les composants principaux : serveur web, serveur d'application et base de données. L'objectif est d'ajouter un serveur supplémentaire et de mettre en place un cluster de load balancers HAProxy.

---

### 🔧 Architecture requise

#### Vous devez ajouter :
- 1 serveur supplémentaire
- 1 load-balancer (HAproxy) configuré en cluster avec le premier
- Composants séparés : serveur web, serveur d’application, base de données sur des machines dédiées

---

### 📚 Explication de l’architecture

- **Serveur supplémentaire** : Ajouté pour améliorer la tolérance aux pannes et permettre la montée en charge horizontale.
- **Cluster HAProxy** : Deux load balancers configurés en haute disponibilité pour éviter un SPOF (Single Point Of Failure).
- **Composants séparés** :
  - **Serveur Web (Nginx)** : Sert les fichiers statiques et gère les requêtes HTTP.
  - **Serveur d’application** : Traite la logique métier.
  - **Base de données (MySQL)** : Stocke les données persistantes.

---

### ✅ Avantages

- Meilleure disponibilité
- Meilleure performance
- Infrastructure prête pour le scaling horizontal

---

## ENGLISH

### Description
This project involves designing a scalable web infrastructure by splitting main components: web server, application server, and database. The goal is to add an extra server and implement a HAProxy load-balancer cluster.

---

### 🔧 Required Architecture

#### You must add:
- 1 additional server
- 1 load-balancer (HAproxy) configured in a cluster with the existing one
- Split components: web server, application server, and database on separate machines

---

### 📚 Explanation of the Architecture

- **Extra Server**: Added to improve fault tolerance and support horizontal scaling.
- **HAProxy Cluster**: Two load balancers configured in high-availability mode to eliminate a single point of failure (SPOF).
- **Split Components**:
  - **Web Server (Nginx)**: Serves static files and handles HTTP requests.
  - **Application Server**: Processes the business logic.
  - **Database (MySQL)**: Stores persistent data.

---

### ✅ Benefits

- Better availability
- Improved performance
- Infrastructure ready for horizontal scaling
