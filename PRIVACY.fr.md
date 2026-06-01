# Politique de confidentialité

**Charty** est publié par Pascal Peltriaux.

**Date d'effet :** 1 juin 2026

---

## En bref

Charty ne collecte rien. Pas de comptes. Pas d'analytique. Pas de publicités. Pas de SDK tiers. Vos données restent sur votre appareil.

---

## Quelles données sont collectées

**Aucune.** Charty ne collecte, ne stocke ni ne transmet aucune donnée personnelle, donnée d'utilisation ou identifiant d'appareil vers un quelconque serveur.

Concrètement, Charty **ne** :

- crée pas de compte utilisateur ;
- ne suit pas l'utilisation, le comportement ou les interactions ;
- n'affiche pas de publicités ;
- n'utilise pas de SDK d'analytique tiers (Google Analytics, Firebase, Mixpanel, etc.) ;
- ne contient aucun pixel de suivi ;
- ne fait aucune requête réseau pour télémétrie, rapport de plantage ou « phone-home » ;
- ne vend, n'échange ni ne partage de données avec qui que ce soit (parce qu'il n'y a aucune donnée à partager).

Cela est garanti par la sandbox iOS d'Apple et par l'absence de tout code réseau ou SDK tiers dans l'application. Vous pouvez le vérifier sur la fiche App Store : sous « Confidentialité de l'app », Charty déclare « Aucune donnée collectée ».

## Ce qui reste sur votre appareil

Charty stocke les éléments suivants localement, sur votre iPhone/iPad, en utilisant le framework SwiftData d'Apple :

- les routines, tâches et plannings que vous créez ;
- le prénom de votre enfant et (en option) une image d'avatar que vous choisissez ;
- les récompenses que vous définissez et le solde de points actuel ;
- l'historique des sessions (quelles routines ont été complétées, quand, points gagnés) ;
- les préférences (son, vibrations, animations, hash du code parental, préférence biométrique) ;
- les photos personnalisées de tâches, si vous choisissez d'en ajouter depuis votre photothèque.

Tout ceci reste sur votre appareil. Rien ne quitte votre appareil sauf si **vous** l'exportez explicitement.

## Choses que vous pouvez faire qui impliquent que des données quittent l'app

Les fonctionnalités suivantes confient les données à **iOS lui-même**, qui les achemine ensuite sous votre contrôle. Charty ne voit jamais ni ne stocke le résultat :

- **Imprimer ou partager en PDF** — Charty génère un PDF localement et présente la feuille de partage iOS. Vous décidez si vous voulez utiliser AirPrint, enregistrer dans Fichiers, envoyer par e-mail, par messagerie, etc.
- **Exporter les sessions en CSV** — Même schéma : fichier généré localement, feuille de partage qui le confie à l'app de votre choix.
- **Synchronisation iCloud** (optionnelle, désactivée par défaut) — Lorsqu'elle est activée dans Réglages, vos données se synchronisent via la **base de données privée** de CloudKit, chiffrée par Apple et liée à votre propre compte iCloud. Le développeur de Charty ne peut pas lire votre base de données privée iCloud. La synchronisation est facultative.

## Confidentialité des enfants

Charty est conçu pour les enfants, principalement de 4 à 10 ans, y compris les enfants présentant des troubles du développement comme le trouble du spectre de l'autisme (TSA).

Nous respectons COPPA (États-Unis) et le RGPD-K (UE) **par conception** : nous ne collectons aucune donnée — ni d'enfants, ni d'adultes — donc il n'y a rien à consentir, rien à traiter, rien à supprimer.

Le verrou parental (code à 4–6 chiffres ou Face ID / Touch ID) garantit que seuls les adultes peuvent modifier les Réglages, éditer les routines ou réinitialiser le solde de points.

## Appareil photo et Photos

Si vous touchez « Choisir une photo » pour une icône de tâche ou pour la récompense puzzle image, iOS affiche son sélecteur de photos standard. La photo choisie est **copiée** dans la sandbox locale de l'app (redimensionnée et compressée en JPEG pour le cas du puzzle). Les photos ne quittent jamais votre appareil.

Charty ne demande pas l'accès à l'appareil photo. Si vous voulez utiliser une photo fraîche, prenez-la d'abord avec l'app Photos puis sélectionnez-la via le sélecteur de photos.

## Face ID / Touch ID

Si vous activez le déverrouillage biométrique pour le verrou parental, l'authentification est entièrement gérée par le système local Face ID / Touch ID d'Apple. Les données biométriques ne quittent jamais le Secure Enclave de votre appareil, et Charty ne les voit jamais — nous recevons uniquement un retour « succès » ou « échec » de la part d'iOS.

## Notifications

Charty planifie des notifications **locales** pour les rappels de routines quotidiennes. Elles sont gérées par iOS et n'impliquent aucun serveur. Vous pouvez les désactiver par routine, ou globalement via Réglages iOS → Notifications → Charty.

## Accès réseau

Charty **ne fait** aucune requête réseau, à l'exception de la synchronisation iCloud si vous l'avez explicitement activée (qui passe par la propre infrastructure iCloud d'Apple). L'application n'a pas d'URL intégrée, pas de point de télémétrie, pas de configuration distante, pas de SDK de pub, pas de SDK d'analytique, pas de rapporteur de plantage. En mode Avion, Charty fonctionne à l'identique (la synchronisation iCloud est simplement mise en pause jusqu'à ce que la connexion revienne).

## Achats

Charty est gratuit à télécharger, avec un déblocage unique facultatif, « Charty Plus ». Les achats sont gérés **entièrement par l'App Store / StoreKit d'Apple** — Charty ne voit jamais votre nom, votre carte bancaire ni votre identifiant Apple. L'application ne stocke qu'un indicateur local indiquant si Plus est débloqué ; cet indicateur est dérivé du reçu Apple sur l'appareil et, si vous activez la synchronisation iCloud, peut transiter par votre propre base iCloud privée. Aucune donnée d'achat ou de paiement n'est collectée par Charty ni envoyée à son développeur. La déclaration « Aucune donnée collectée » de l'App Store reste valable.

## Modifications de cette politique

Si cette politique change, la nouvelle version remplace ce fichier dans le dépôt public. Les changements importants seront notés en haut avec une nouvelle date d'effet. Comme aucune donnée n'est collectée, il n'y a pas de données historiques à migrer ou à réutiliser.

## Contact

📧 **E-mail :** dev@peltriaux.com

Questions, préoccupations ou demandes de vérification indépendantes bienvenues.
