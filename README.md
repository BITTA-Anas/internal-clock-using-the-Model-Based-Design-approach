# Création d'une Horloge Interne avec l'Approche Model-Based Design (MBD)

Ce projet a été réalisé dans le cadre d'un stage d'initiation en Génie des systèmes embarqués. L'objectif principal est la conception et l'implémentation d'une horloge interne capable de gérer la date et l'heure, en utilisant la méthodologie **Model-Based Design (MBD)** avec MATLAB et Simulink.

Ce dépôt contient les modèles Simulink, les scripts de test, les rapports de couverture de code et le code C généré automatiquement.

---

## 📖 Contexte du Projet

Le projet a été développé au sein de l'entreprise **ALTEN Fès**, un leader en ingénierie et conseil technologique, spécialisé notamment dans le secteur automobile.

L'objectif était de développer une fonctionnalité d'horloge interne robuste, une composante essentielle dans de nombreux systèmes embarqués, où la précision et la fiabilité temporelles sont cruciales. L'approche MBD a été choisie pour sa capacité à modéliser, simuler, valider et générer automatiquement le code, réduisant ainsi les erreurs et le temps de développement.

- **Université :** Université Privée de Fès (UPF)
- **Entreprise d'accueil :** ALTEN Fès
- **Auteur :** BITTA Anas
- **Encadrant :** KARAME Youssef

---

## 🎯 Objectifs

L'objectif principal est de développer une horloge interne en utilisant l'approche Model-Based Design. Cette horloge doit :

1.  **Suivre la date et l'heure actuelles** (année, mois, jour, heure, minute).
2.  Permettre à l'utilisateur de **modifier dynamiquement l'heure** en ajoutant ou soustrayant des heures.
3.  **Gérer automatiquement les transitions** de jours, de mois et d'années, y compris la gestion des **années bissextiles**.
4.  Générer du **code C portable et fiable** à partir du modèle validé, en respectant les normes de l'industrie comme MISRA C.

---

## 🛠️ Méthodologie et Outils

### Approche de Conception
Le projet suit rigoureusement le cycle de vie du **Model-Based Design (MBD)** :
1.  **Définition des exigences :** Spécification des besoins fonctionnels et non fonctionnels.
2.  **Modélisation :** Création de modèles comportementaux avec Simulink.
3.  **Simulation et Validation :** Tests du modèle dans diverses conditions pour corriger les erreurs en amont.
4.  **Génération de code :** Production automatique de code C à partir du modèle.
5.  **Vérification :** Tests unitaires et de couverture de code (MC/DC) pour garantir la robustesse.

### Outils Utilisés
- **MATLAB :** Pour les scripts, les fonctions logiques et l'analyse.
- **Simulink :** Pour la modélisation graphique, la simulation et les tests du système.
- **Simulink Test :** Pour la création de *Test Harness* et l'automatisation des scénarios de test.
- **Simulink Coverage :** Pour mesurer la couverture de code (décision, condition, MC/DC).
- **Embedded Coder :** Pour la génération de code C optimisé pour les systèmes embarqués.

---

## 📂 Structure du Dépôt

- `slprj/` : Contient les fichiers de projet Simulink et les artefacts de compilation.
- `slcov_output/` : Contient les rapports de couverture de code générés après les tests.
- `report_internal_clock_3_3/` : (Optionnel) Pourrait contenir le rapport de stage ou la documentation détaillée.
- `Horloge_interne_v3.slx` : Le fichier principal du modèle Simulink.
- `Horloge_interne_v3_test.mldatx` : Fichier de données de test pour le modèle.
- `*.c`, `*.h` : Fichiers de code source C et en-têtes générés par Embedded Coder.

---

## 🚀 Comment Utiliser

1.  **Prérequis :** Assurez-vous d'avoir MATLAB, Simulink, Simulink Test et Embedded Coder installés.
2.  **Ouvrir le projet :** Lancez le fichier `internal-clock-using-the-Model-Based-Design-approach.prj` pour configurer l'environnement MATLAB.
3.  **Explorer le modèle :** Ouvrez le fichier `Horloge_interne_v3.slx` pour voir l'architecture du système.
4.  **Exécuter les tests :** Ouvrez le gestionnaire de tests Simulink pour lancer les scénarios de validation et générer les rapports de couverture.
5.  **Générer le code :** Utilisez Embedded Coder à partir du modèle pour générer le code C.

