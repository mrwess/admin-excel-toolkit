<div align="center">

# 🩺 Suivi des certificats médicaux — Bureau d'ordre

**Classeur Excel bilingue (français · عربي) pour suivre, mois par mois, les certificats médicaux du personnel d'un établissement universitaire.**

[![Licence CC BY-NC 4.0](https://img.shields.io/badge/licence-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Usage commercial](https://img.shields.io/badge/usage%20commercial-interdit-red)](#-licence-et-conditions-dutilisation)
[![Excel](https://img.shields.io/badge/Excel-2010%2B-217346?logo=microsoftexcel&logoColor=white)](#-prérequis)
[![LibreOffice](https://img.shields.io/badge/LibreOffice-compatible-18A303?logo=libreoffice&logoColor=white)](#-prérequis)
[![Langues](https://img.shields.io/badge/langues-FR%20%7C%20AR-0F7B8A)](#-fonctionnalités)
[![Sans macros](https://img.shields.io/badge/macros-aucune-lightgrey)](#-prérequis)
[![Version](https://img.shields.io/badge/version-1.0.0-1B365D)](https://github.com/VOTRE-UTILISATEUR/admin-excel-toolkit/releases)

[⬇️ Télécharger le modèle](Suivi_Certificats_Medicaux_Modele.xlsx) · [Mode d'emploi](#-mode-demploi) · [Personnalisation](#-personnalisation) · [FAQ](#-faq)

</div>

---

> **بالعربية:** مصنف Excel ثنائي اللغة (عربي/فرنسي) لمتابعة الشهادات الطبية الواردة على مكتب الضبط بالمؤسسات الجامعية، مع إحصائيات شهرية وسنوية آلية وربط بمرجع منظومة إنصاف. الاستعمال التجاري ممنوع.

## 📌 Aperçu

Ce classeur aide l'agent(e) du bureau d'ordre à **enregistrer chaque certificat médical reçu**, à suivre la **saisie de la référence dans INSAF** et à obtenir **automatiquement les statistiques** du mois et de l'année.

Il est autonome : **aucune macro, aucune installation, aucune connexion**. Il suffit d'ouvrir le fichier dans Excel.

<p align="center">
  <img src="img/accueil.png" width="40%" alt="Page d'accueil et navigation">
  &nbsp;
  <img src="img/mois.png" width="57%" alt="Feuille mensuelle avec statistiques">
</p>
<p align="center">
  <img src="img/synthese.png" width="49%" alt="Synthèse annuelle et graphiques">
  &nbsp;
  <img src="img/par-agent.png" width="49%" alt="Suivi annuel par agent">
</p>

<sub>Captures réalisées avec des **données fictives**.</sub>

## ✨ Fonctionnalités

- 🗓️ **12 feuilles mensuelles** + synthèse annuelle + suivi par agent
- 🌐 **Bilingue** : en-têtes, libellés, bulles d'aide et messages d'erreur en français et en arabe
- 👤 **Saisie guidée** : l'agent se choisit dans une liste, ses informations (nom, prénom, identifiant, grade/poste) se remplissent seules
- 📅 **Calculs automatiques** : date de fin, date de reprise
- 🏷️ **Suivi INSAF** : statut par ligne — ✔ Saisi · ○ À saisir · ⚠ Incomplet
- 📊 **Statistiques en temps réel** : certificats reçus, agents concernés, total de jours, durée moyenne, part de l'effectif, avancement de la saisie INSAF
- 📈 **Vue annuelle** : tableau mois par mois, 2 graphiques, matrice agents × mois avec carte de chaleur
- 🛡️ **Contrôles de saisie** : dates cohérentes avec le mois, durée entre 1 et 365 jours, agent obligatoirement choisi dans la liste, identifiant sur 10 chiffres sans doublon
- 🔒 **Feuilles protégées** (sans mot de passe) : seules les cellules jaunes sont modifiables
- 🖨️ **Prêt à imprimer** : A4 paysage, en-têtes répétés, pagination, bloc de signatures pour la clôture mensuelle
- 🎨 **Zones de logos** dans l'en-tête de chaque feuille

## 🧭 Structure du classeur

| Onglet | Rôle |
|---|---|
| **Accueil** | Guide en 5 étapes, légende, exemple de saisie, historique des versions, boutons de navigation |
| **Paramètres** | Établissement (FR/AR), année, effectif, code et version du document, liste du personnel (capacité maximale : 40 agents) |
| **Janvier → Décembre** | Registre mensuel : saisie, statuts INSAF, statistiques du mois, signatures de clôture |
| **Synthèse** | Totaux par mois, indicateurs de l'année, graphiques |
| **Par agent** | Jours de congé par agent et par mois, total et nombre de certificats |
| **À propos** | Auteur, version, licence et conditions d'utilisation |

## 🚀 Prérequis

- Microsoft Excel 2010 ou plus récent (Windows, macOS) — ou LibreOffice Calc
- Aucune macro : le fichier est en `.xlsx`
- Si Excel affiche une barre jaune « Mode protégé », cliquer sur **Activer la modification**

## 📘 Mode d'emploi

### 1. Préparer le classeur (une seule fois)

1. Ouvrir l'onglet **Paramètres**.
2. Renseigner l'établissement (version française et arabe), l'**année**, l'**effectif**, le **code** et la **version** du document, la **date d'application**.
3. Saisir la **liste du personnel** : nom, prénom, identifiant unique, grade/poste.
   - L'identifiant est numérique : taper `65961010` affiche `0065961010` (10 chiffres, zéros ajoutés automatiquement).
   - Chaque identifiant doit être unique.
4. *(Facultatif)* Ajouter les logos — voir [Personnalisation](#-personnalisation).

### 2. À chaque certificat reçu

1. Ouvrir l'onglet du **mois d'arrivée** (ex. *Janvier*).
2. Prendre la première ligne vide et remplir les **cellules jaunes** :
   - **Date d'arrivée** (doit appartenir au mois) et **n° d'ordre**
   - **Agent** (liste déroulante)
   - **Début du congé**, tel qu'inscrit sur le certificat, et **durée en jours**
3. Les **cellules grises** se remplissent seules : nom, prénom, identifiant, grade, date de fin, reprise, statut.

### 3. En fin de mois

1. Saisir dans la colonne **Réf. INSAF** la référence de chaque certificat, depuis l'application INSAF. Le statut passe à **✔ Saisi**.
2. Consulter les **statistiques** en haut de la feuille.
3. Remplir la date de clôture, imprimer si besoin et faire signer le bloc **Établi par / Vérifié par / Approuvé par**.

### 4. Suivi annuel

- **Synthèse** : vue d'ensemble des 12 mois et graphiques.
- **Par agent** : cumul des jours et nombre de certificats par agent, avec carte de chaleur.

### Code des couleurs

| Couleur | Signification |
|---|---|
| 🟨 Jaune clair | Cellule à saisir |
| ⬜ Gris clair | Cellule automatique — ne pas modifier |
| 🟩 Vert | ✔ Saisi : référence INSAF renseignée |
| 🟧 Orange | ○ À saisir : référence INSAF en attente |
| 🟥 Rouge | ⚠ Incomplet : agent, date ou durée manquants |

## 🎛️ Personnalisation

### Ajouter les logos

Les feuilles de suivi sont protégées **sans mot de passe**.

1. Onglet **Révision** › **Ôter la protection de la feuille**.
2. **Insertion** › **Images** › choisir le logo.
3. Ajuster l'image dans la zone en pointillés.
4. Ordre prévu, de gauche à droite : **Établissement · République · Université**.
5. Pour gagner du temps entre les 12 feuilles mensuelles (même disposition) : sélectionner l'image, `Ctrl+C`, ouvrir l'autre feuille, cliquer sur la cellule `A2`, `Ctrl+V`.

Les textes de l'en-tête (République, ministère, université, établissement) se modifient dans **Paramètres** et se répercutent sur tous les onglets.

### Changer l'année

Modifier la cellule **Année civile** dans **Paramètres** : les 12 feuilles se mettent à jour. Pour une nouvelle année, enregistrer le classeur sous un nouveau nom et vider les lignes de saisie.

## ⚙️ Règles de calcul

- Chaque certificat est rattaché au **mois de son arrivée** au bureau d'ordre.
- Les durées sont comptées en **jours calendaires**.
- *Part de l'effectif* = agents concernés ÷ effectif de référence.
- Capacité maximale : **60 certificats par mois** et **40 agents**.

## ❓ FAQ

**Je ne peux pas modifier une cellule.**
Elle est protégée : seules les cellules jaunes sont modifiables. Pour une adaptation de la mise en page, ôter la protection de la feuille (Révision), sans mot de passe.

**Je ne peux pas ajouter, supprimer ou renommer un onglet.**
La structure du classeur et l'onglet **À propos** sont protégés par mot de passe afin de préserver la mention de l'auteur. Les feuilles de saisie restent entièrement utilisables.

**La liste des agents est vide dans la feuille du mois.**
Vérifier que les identifiants sont renseignés dans **Paramètres** : seuls les agents ayant un identifiant apparaissent dans la liste.

**Un agent ne se trouve pas dans la liste.**
L'ajouter dans **Paramètres** (jusqu'à 40 agents).

**Comment archiver l'année ?**
Enregistrer une copie du classeur en `.xlsx` et, si nécessaire, exporter les feuilles en PDF.

## 🔐 Données personnelles

Ce dépôt ne contient **aucune donnée réelle** : la liste du personnel est vide et aucun logo n'est fourni.

Une fois le classeur rempli, il contient des données personnelles relatives à l'absence du personnel. Appliquer les règles de protection des données en vigueur dans votre établissement : accès restreint, sauvegarde sécurisée, **ne jamais publier un classeur rempli**.

## 📄 Licence et conditions d'utilisation

Ce travail est distribué sous licence **[Creative Commons Attribution – Pas d'Utilisation Commerciale 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/)**. Voir le fichier [LICENSE](../../LICENSE).

| ✅ Autorisé | ❌ Interdit |
|---|---|
| Utiliser le classeur dans un établissement public, une administration ou une association à but non lucratif | Vendre le classeur ou l'inclure dans une offre payante |
| Le copier, le partager et l'adapter à vos besoins | Toute exploitation commerciale, directe ou indirecte |
| Le modifier et le redistribuer, **en citant l'auteur** et en indiquant les modifications | Retirer la mention de l'auteur |

## 🤝 Contribuer

Les suggestions sont les bienvenues : ouvrez une *issue* pour signaler une anomalie ou proposer une amélioration. Les adaptations à d'autres établissements ou à d'autres systèmes de gestion des ressources humaines sont encouragées, dans le respect de la licence.

## ✍️ Auteur

**Wissem Zeddini**
📫 [zdiniwissem@yahoo.fr](mailto:zdiniwissem@yahoo.fr)

---

<div align="center">

*Fait pour simplifier le quotidien des bureaux d'ordre universitaires.*
<br>
© 2026 Wissem Zeddini · CC BY-NC 4.0

</div>
