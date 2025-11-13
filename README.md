#  TP Site — Déploiement Automatique sur o2switch

![Deploy](https://github.com/pokam-dev/site/actions/workflows/deploy-api.yml/badge.svg)

Ce site est déployé automatiquement sur o2switch à chaque push sur la branche **main**.  
Lien du site : 👉 [https://tp.p-wf.fr](https://tp.p-wf.fr)

---

## Fonctionnement

1. Quand je fais un `git push`, GitHub exécute le fichier **.github/workflows/deploy-api.yml**.
2. Ce fichier envoie automatiquement mon site sur le serveur o2switch.
3. cPanel exécute le script **.cpanel.yml** pour copier les fichiers vers :  
   `/home/Mon_ID/public_html/tp`
4. Le site est ensuite visible immédiatement sur [https://tp.p-wf.fr](https://tp.p-wf.fr)

---

##  Structure du projet

```bash
.
├── index.html
├── Style.css
├── img/
├── .github/
│   └── workflows/
│       └── deploy-api.yml   # (tâches CI/CD)
└── .cpanel.yml              # (script de déploiement côté o2switch)


---

##  Auteur

**p-wf**  
Projet de déploiement automatique d’un site statique sur o2switch.


