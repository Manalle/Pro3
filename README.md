# Projet PRO3 – Atelier DevOps 🐳

## Description

Projet réalisé dans le cadre de l’atelier L3 MIAGE DevOps animé par [Nicolas Lebacq](https://github.com/SmashingQuasar).

---

## Membres du groupe

Oumlil Manal et Xynou Eleni

---

## Prérequis

- **Docker Desktop**
- Être sous **Linux / WSL / Debian / Ubuntu**
- Navigateur web (Chrome, Firefox, ...)

---

## ⚙️ Étapes pour exécuter le projet

### Étape 1 : Démarrer le service Docker

```bash
./up.sh
```

---

### Étape 2 : Accéder à l'application

Dans votre navigateur ou via curl :

```bash
curl -k http://localhost:80
```

Ou ouvrez [http://localhost](http://localhost) dans un navigateur.  
Vous verrez un message du type : `Hello, world!`

---

### Étape 3 : Arrêter le service

```bash
./down.sh
```

---

## 📂 Arborescence du projet

```
Pro3/
├── apps/
│   └── main.mjs                   
├── _ops/
│   ├── scripts/                   
│   │   ├── up.sh
│   │   └── down.sh
│   └── services/
│       └── node/
│           ├── docker-compose.yaml
│           ├── Dockerfile
│           ├── files/
│           │   └── .env
│           └── scripts/
│               └── entrypoint.sh 
```

---


