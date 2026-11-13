# Réseaux informatiques · Infrastructure digitale

Application web pour les stagiaires OFPPT de 1re année (Infrastructure digitale) :
Page d'accueil (présentation de la filière Infrastructure Digitale) puis cinq modules (menu en haut du site) : Conception d'un réseau informatique (8 thèmes, 33 leçons, labs VLAN, QCM de fin de chapitre), Automatiser les tâches d'administration (Bash, PowerShell, Python : 9 leçons, 6 TP), Veille technologique (9 leçons) Sécurité informatique (9 leçons, 6 TP) et Bases de la cybersécurité (11 leçons, 10 labs, 6 études de cas). Les modules Automatisation et Sécurité sont verrouillés (contenu chiffré, accès formateur). Chaque leçon a une fiche de cours, une simulation et un QCM corrigé ; chaque module a un QCM de 10, 20 ou 40 questions.

Site en ligne : https://infrastructure-digitale.netlify.app/

## Organisation
- Thème « Le routage statique et dynamique » (leçons 48 à 51) avec les simulations `simLookup`, `simStatic`, `simDyn`.
- QCM de fin de chapitre : objet `CHAPQ` (15 questions par chapitre).
- Module Automatisation (leçons 52 à 60, chapitres 10 à 12) : simulateurs `simTerm` (terminal à missions), `simTrace` (exécution pas à pas), `simCron` ; cours `automatisation.html`, PDF `docs/automatisation-administration.pdf`.
- Module Cybersécurité (leçons 61 à 71, chapitres 13 à 15) : simulateurs `simUrl`, `simRansom`, `simSqli`, `simLayers`, `simSpot` ; cours `cybersecurite.html`, PDF `docs/bases-cybersecurite.pdf`.
- Menu des modules : tableau `MODULES` (lien direct : `index.html#accueil`, `#m103`, `#auto`, `#veille`, `#secu`, `#cyber`).
- Cours complets en HTML : `veille.html`, `securite.html` (TP et solutions : `securite.html#tp`) ; PDF dans `docs/`.
- Simulations ajoutées : `simOrder`, `simRisk`, `simPhish`, `simPwd`, `simHash`, `simHarden`, `simAcl`, `simWifi`, `simBackup`, `simQuery`, `simCraap`.

Le thème « La veille technologique » (leçons 30 à 38) couvre le cycle de veille, les sources, les outils, la méthode CRAAP, l'organisation, la diffusion, le cadre légal et le projet de veille. Chaque leçon a une simulation de mises en situation (`pick`) et renvoie vers le cours complet en PDF : `docs/veille-technologique.pdf`.

Le site utilise un thème bleu nuit, sarcelle et or (polices Lora et Inter), en mode clair et sombre, adapté au mobile.

Le thème « La redondance des réseaux » (leçons 27 à 29) couvre les atouts de la redondance, STP et VRRP, avec les simulations `simRedund`, `simStp` et `simVrrp`.

Tout le site tient dans `index.html` (HTML, CSS et JavaScript, sans dépendance à installer).
- Les leçons sont dans le tableau `THEMES`, les thèmes dans `CHAPS` et `CLEAD`.
- Chaque simulation est une fonction déclarée dans `SIMS`.
- Le thème « Les VLAN » ajoute `simVlanBc` (diffusion), `simLab` (lab interactif) et l'onglet Lab (`labTabHTML`).

## Publication
Le dépôt est relié à Netlify : chaque modification poussée sur la branche `main`
est publiée automatiquement (fichier `netlify.toml`, aucune étape de build).
