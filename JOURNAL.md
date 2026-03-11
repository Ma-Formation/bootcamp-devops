# 📖 Journal de Bord DevOps - Bootcamp Ansible & Terraform

## 🎯 Pourquoi je fais ce bootcamp
Mon objectif principal en rejoignant cette formation est d'acquérir une expertise technique pointue sur **Ansible**. Je souhaite consolider mes compétences pour être rapidement opérationnel et hautement employable sur des postes d'ingénieur DevOps.

## 🚀 Ma vision à 12 semaines
D'ici 12 semaines, je vise l'excellence opérationnelle sur **Terraform** et **Ansible**. Mon ambition est d'atteindre un niveau de maîtrise avancé qui me permettra de concevoir, gérer et dépanner les architectures les plus critiques, de manière autonome et dans n'importe quel environnement technique.

---

## 📅 Jour 1 : Fondations et premier contact

### 📝 Ce que j'ai accompli ce soir :
* **Mise en place de l'environnement :** Configuration et validation de la connectivité SSH entre mon environnement local (Mac) et ma machine virtuelle (Rocky Linux).
* **Configuration d'Ansible :** Création du fichier d'inventaire `hosts.ini` et paramétrage du fichier de configuration principal `ansible.cfg`.
* **Sécurité et clés SSH :** Gestion du paramètre `host_key_checking` pour fluidifier et sécuriser la connexion aux hôtes.
* **Validation technique :** Exécution réussie de ma première commande ad-hoc (`ansible all -m ping`) pour tester la communication avec l'infrastructure.
* **Théorie appliquée :** Compréhension et validation sur le terrain du concept clé d'**idempotence**, pilier de l'automatisation avec Ansible.

### 🐛 Erreurs rencontrées et leçons apprises :
* **Résolution des chemins relatifs :** Confusion sur le répertoire de travail entre `ansible/inventories/...` et `inventories/...`. J'ai bien compris l'importance de savoir d'où la commande `ansible` est exécutée.
* **Syntaxe des chemins absolus :** Omission du `/` racine dans la définition d'un chemin absolu, ce qui faussait la localisation du fichier d'inventaire par Ansible.
* **Blocage SSH (Known Hosts) :** Définition erronée de `host_key_checking = True` au lieu de `False` dans `ansible.cfg`. Cela bloquait l'authentification silencieuse lors de la première connexion à la VM. J'ai corrigé ce paramètre pour fluidifier les tests en environnement de développement.

### ✅ Checklist de fin de session :
- [x] Entrée du Jour 1 complétée dans le `JOURNAL.md`.
- [x] Code et configurations sauvegardés (`git commit` + `git push`).
