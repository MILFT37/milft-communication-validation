# MAJ 35 — Correction de l'environnement CI navigateur

**25/11/2026 — V0.29 inchangée.**

- Exécution navigateur 45565684728 : échec avant recette, à l'installation Playwright 1.56.1 incompatible avec Ubuntu 26.04 sélectionné par ubuntu-latest (journal job 139039764874). Aucun défaut applicatif démontré.
- Correction ciblée : ubuntu-24.04, commit 7c7c0548f758914ca8af781e2a0374b1316a6b05. Nouvelle exécution à vérifier. État au dernier contrôle : [{"name":"Recette navigateurs MILFT Communication","id":45566686125,"status":"in_progress","conclusion":null},{"name":"Validation MILFT Communication","id":45566686090,"status":"in_progress","conclusion":null},{"name":"pages build and deployment","id":45566685953,"status":"in_progress","conclusion":null},{"name":"Validation MILFT Communication","id":45565705594,"status":"completed","conclusion":"success"},{"name":"pages build and deployment","id":45565705593,"status":"completed","conclusion":"success"}].
- Recette Samsung courte déjà validée, ne pas la recommencer. Recette complète groupée : deux joueurs fictifs, export qualité MP4 720p puis 1080p, lecture/téléchargement, PNG, sauvegarde/restauration et persistance après fermeture. Aucun GO intermédiaire. Pas de données réelles ni production.

---

# MAJ 34 — Première recette Samsung et CI navigateur

**25/11/2026 — prototype V0.29 inchangé.**

- Retour utilisateur « C'est tout bon go » après ouverture HTTPS, diagnostic, test court et lecture/téléchargement vidéo sur Samsung. Ces opérations sont validées par l'utilisateur ; rapport JSON et fichier MP4 non reçus, résolution et cadence non mesurées indépendamment. Ne pas recommencer ce test court sans motif.
- CI statique 45565369199 et Pages 45565367953 verts.
- Workflow navigateur `.github/workflows/browser-validation.yml` ajouté au commit `24896f4409ae9de97b50498e45774734a95ce337` : chargement Chromium desktop/mobile et WebKit mobile émulé, erreurs JS, canvas, stockage temporaire, PNG, relevé capacités codec. Résultats à vérifier ; ne remplace pas les appareils physiques ni le montage MP4 réel.
- Recette Samsung restante à regrouper : montage fictif avec deux joueurs, export MP4 complet (720p puis 1080p), PNG, sauvegarde/restauration JSON et persistance après fermeture. Windows/iPhone ensuite. Ne pas utiliser les données réelles ; graphismes, animation et son inchangés. Aucun GO intermédiaire.

---

# MAJ 33 — Déploiement de validation réussi

**25/11/2026 — V0.29 inchangée.**

- Déploiement GitHub Pages [45564956466](https://github.com/MILFT37/milft-communication-validation/actions/runs/45564956466) terminé avec succès : build, deploy, report-build-status verts ; premier déploiement remplacé par celui-ci. CI [45564956513](https://github.com/MILFT37/milft-communication-validation/actions/runs/45564956513) verte.
- Adresse de validation : https://milft37.github.io/milft-communication-validation/ . Ouverture directe non accessible depuis l'outil web de la session ; chargement sur Samsung restant à vérifier. Aucun changement du HTML ni publication de production.
- Intervention nécessaire : ouvrir l'adresse dans Chrome sur Samsung, lancer le diagnostic local puis le test vidéo court MP4, contrôler lecture et téléchargement, transmettre résultats/capture. Ensuite montage fictif et recette groupée ; Windows/iPhone à suivre. Ne pas redemander de GO entre étapes autonomes. Retour utilisateur : « Trop de go ».

---

# MAJ 32 — Activation de l’hébergement de validation

**25/11/2026 — V0.29 inchangée.**

- Activation GitHub Pages réalisée par l'utilisateur depuis Samsung : métadonnée `has_pages=true` confirmée. Deux exécutions CI statique réussies (45564440703 et 45564509211).
- Premier déploiement [45564874642](https://github.com/MILFT37/milft-communication-validation/actions/runs/45564874642) déclenché ; compilation Jekyll en cours au dernier contrôle. URL HTTPS attendue : https://milft37.github.io/milft-communication-validation/ ; accès direct non vérifiable via l'outil web à ce stade. Ne pas déclarer le déploiement réussi avant confirmation.
- Aucune modification du prototype. Pas de production. Suite : vérifier la fin du déploiement puis recette groupée Samsung (diagnostic, test court, montage fictif), Windows et iPhone. Aucun GO développement requis ; intervention appareil seulement après disponibilité du site.

---

# MILFT Communication — MAJ 31

**25/11/2026 — validation distincte uniquement ; V0.29 inchangée.**

- Workflow `.github/workflows/validation.yml` installé au commit `6f6561190a14a792e15ee35a6874f06ab0e3ae0f`. Contrôle structure HTML/canvas, présence VideoEncoder/VideoFrame/localStorage, syntaxe Node de tous les scripts JavaScript intégrés détectés.
- Première exécution [45564440703](https://github.com/MILFT37/milft-communication-validation/actions/runs/45564440703), job 139035697250 : toutes les étapes terminées avec succès. Contrôle statique seulement ; aucun test natif MP4, stockage réel ou appareil effectué.
- Métadonnées GitHub : dépôt public, branche main, Pages non activé (has_pages=false). Le connecteur ne fournit pas d'action d'activation Pages ; endpoint de lecture Pages non autorisé. Intervention indispensable : dans Settings > Pages, sélectionner Deploy from a branch, main, /(root), Save. Hébergement de validation déjà autorisé, pas de production.
- Suite : vérifier déploiement HTTPS et accès au prototype puis recette groupée Samsung, avant Windows/iPhone. Aucun nouveau GO développement. Ne pas entrer de données réelles ; animation et son reportés. Ne pas toucher aux autres dépôts.

---

# MILFT Communication — Reprise MAJ 30

**25/11/2026 — validation uniquement ; prototype V0.29 inchangé.**

- Autorisation du dépôt de validation distinct accordée avant interruption du chat.
- Dépôt `MILFT37/milft-communication-validation`, branche `main`. Import confirmé au commit `2e5697189357ce3f5d02d33d687d9f6fd7e6c778` : `index.html`, 2 174 862 octets, blob `0450b7fa359488587544a1a27f95c4a647fd8972`. La taille correspond au fichier V29 en bibliothèque ; comparaison des octets non effectuée.
- À la reprise : aucun workflow enregistré ni exécution constatée. HTTPS et recette réelle non confirmés.
- Suite : installer la CI de validation, vérifier HTTPS, puis recette groupée Samsung (diagnostic + test vidéo court, puis montage réel), Windows et iPhone. Pas de production ni de données réelles ; animations et son reportés. Aucun GO intermédiaire.
- Historique intégral disponible ci-dessous, récupéré sous forme de texte depuis la feuille MAJ29 (pas une copie binaire).

---

# MILFT Communication — Feuille de route et dossier de reprise

**MAJ 29 | 25/11/2026 | Reprise de la V0.28**  
**Version de travail : V0.29 Arena — prototype, non publié.**  
**Règle : ce document est la référence de reprise ; mettre à jour après chaque avancée significative.**

## 0I. MAJ29 — point de reprise prioritaire

- FN-03/FN-07 : test vidéo court indépendant du projet, deux secondes et 60 images horodatées, à la résolution sélectionnée, dans un canvas séparé, via le même exporteur H.264/MP4 que les montages. Lecture intégrée, téléchargement et rapport de diagnostic enrichi, annulation et libération des contrôles. Protection contre une file d'encodage ou finalisation bloquée (20 s). Graphismes et ressources inchangés. Le test court ne vaut pas validation d'un montage réel.
- Contrôles : syntaxe Node OK ; dix assertions Playwright réussies (assets, refus d'encodeur indisponible, pipeline 60 images simulé, projet/bibliothèque intacts, contrôles, téléchargement, rapport, annulation, invalidation manuelle du format, pas d'exception JS). MP4 de preuve obtenu à partir d'échantillons préencodés, ffprobe H.264 720×1280, 60 images, 30 i/s, 2 s, décodage ffmpeg sans erreur. Ce fichier de preuve n'est pas le rendu du canvas fictif. Navigation HTTPS bloquée par l'environnement (ERR_BLOCKED_BY_ADMINISTRATOR) ; WebCodecs natif et persistance réelle restent non testés. Aucun test réel Samsung, Windows ou iPhone.
- OPS-01 : dossier d'installation HTTPS actualisé, script de vérification statique autonome et workflow GitHub Actions préparés localement ; aucune création de dépôt, aucun envoi ni publication. Le workflow n'a pas été exécuté sur GitHub.
- Prochaine étape indispensable : autorisation explicite d'un hébergement de validation HTTPS distinct de Tournois et Compta (pas de production ni réseaux sociaux). Puis une recette groupée sur Samsung, en commençant par le diagnostic et le test court, avant la recette complète. Finition graphique/animations et son reportés. Ne plus créer de micro-MAJ de préparation sans avancée utile ; GO développement acquis.

## 0H. MAJ28 — point de reprise prioritaire

- FN-07/FN-03 : diagnostic local de compatibilité intégré, vérification du contexte sécurisé, lecture/écriture via clé de stockage temporaire, génération PNG réelle, formats MediaRecorder annoncés et disponibilité de configuration H.264 WebCodecs pour la résolution sélectionnée. Export d'un rapport JSON sans données joueurs, ni réseau, invalidation lors d'un changement de format. Le diagnostic est distinct d'un test d'encodage complet et ne certifie pas la persistance après fermeture.
- Contrôles : syntaxe Node OK ; dix assertions Playwright réussies (assets identiques, dimensions 720p vertical/carré, PNG réel, stockage simulé avec nettoyage, rapport sans données personnelles, téléchargement JSON, invalidation, échec stockage signalé, aucune erreur JS). La configuration WebCodecs native reste à vérifier sur appareil réel. Aucun graphisme modifié.
- Préparation OPS-01 : dossier statique local prêt à héberger sur HTTPS, sans création de dépôt, sans publication. Recette groupée fournie pour les futurs essais Samsung/Windows/iPhone. Pas de décision imposée sur l'hébergeur.
- Retour utilisateur : « Trop de go ». Regrouper les chantiers autonomes et les validations indispensables ; ne demander aucun GO intermédiaire. Ne pas annoncer de traitement hors conversation. Animations non validées et reportées ; bande-son reportée.
- Suite : hébergement HTTPS à préparer dans un dépôt distinct avec autorisation explicite avant publication ; recette réelle groupée incluant export H.264 720/1080, persistance, restauration et lecture du fichier sur Samsung. Pas de mise en production finale avant recette. 

## 0G. MAJ27 — point de reprise prioritaire

- FN-08 : sauvegarde manuelle consolidée du projet actif et de la bibliothèque en un JSON versionné, autonome, photos intégrées. Aucun accès réseau ou envoi automatique ; fichier conservable sur téléphone ou Drive, aucun connecteur ni synchronisation. Les commandes individuelles restent disponibles. Restauration après validation complète du JSON et décodage des images ; confirmation explicite du remplacement du montage ; fusion des joueurs par nom normalisé, doublons locaux conservés. En cas d'échec stockage, bibliothèque en mémoire avec avertissement ; si stockage initial illisible, demande de confirmation pour exporter seulement ce qui est disponible en mémoire. Aucun changement graphique.
- Contrôles exécutés : syntaxe Node OK, dix assertions Playwright réussies : assets identiques, sauvegarde combinée et photo incluse, annulation sans changement, restauration projet, fusion non écrasante, écriture simulée, rejet fichier invalide, échec quota signalé, absence d'erreur JS. Stockage simulé ; pas de garantie de persistance réelle ni de synchronisation Drive. Données fictives exclusivement. 
- Suite : préparer diagnostic de compatibilité et recette FN-07/FN-03 sur Samsung/Windows/iPhone, puis OPS-01 si autorisé. Graphismes et animations joueurs préservés, bande-son et finition animation reportées, pas de publication. GO développement acquis.

## 0F. MAJ26 — point de reprise prioritaire

- FN-06 : gabarits sans photo pour annonce de tournoi, félicitations/performance, podium, communication libre. Type, titre, date/lieu, trois informations dont rangs 1/2/3 pour podium et badge facultatif. Rendu dédié à une publication, couleurs selon modèle et accents de rang ; sélection explicite cartes joueurs / publication. Les anciennes cartes ne sont pas supprimées, les anciennes sauvegardes de type événement gardent le mode cartes par défaut. PNG et timeline avec intro/outro facultatives (intro publication 3,6 s). Les quatre images intégrées sont strictement inchangées ; moteur de dessin joueurs conservé. Ces gabarits sont des propositions, pas une validation esthétique ; pas de nouvelle animation joueur.
- Contrôles exécutés : syntaxe Node OK, 18 assertions Playwright réussies : ressources identiques, sélection et durée, quatre rendus distincts, PNG podium 720×1280/900/720, intro/outro échantillonnées, sauvegarde/restauration, retour cartes intactes et ancien JSON événement, pas d'exception JS. Stockage simulé, export natif vidéo et appareil réel toujours à tester. PNG podium fictif inspecté. Pas de publication ni son.
- Suite : FN-08 sauvegarde manuelle consolidée, préparation FN-07 et OPS-01 sans créer ni publier de dépôt sans autorisation. Animations reportées et non validées, GO développement acquis.

## 0E. MAJ25 — point de reprise prioritaire

- FN-05 : registre de trois préréglages graphiques indépendants du type de communication (`GRAPHIC_MODELS25`) : Arena bâche de référence, Sport portrait épuré, Prestige bleu et or. Chaque préréglage applique exclusivement les paramètres visuels (couleur, ambiance, métal, épaisseur, rails, carte, transition, révélation et tissu). Les valeurs des réglages visuels précédents sont remplacées lors d’un changement volontaire de modèle ; pas de bibliothèque de variantes personnalisées persistantes pour l’instant. Le sélecteur identifie automatiquement un modèle connu ou « Réglages personnalisés ». L’identification est dérivée des paramètres JSON v1, donc pas de champ redondant ni de rupture avec les anciens fichiers. Le contenu du montage, les portraits/cadrages, l’ordre, le logo, le type, le format, la résolution, les durées de carte et d’outro sont préservés ; durée totale susceptible de changer selon intro et transition propres au modèle.
- Les modèles Sport et Prestige réutilisent les moteurs de rendu existants (classic/arena) et sont des propositions non validées. Le registre est une première couche modulaire, pas un nouveau moteur de rendu ni une bibliothèque complète de créations graphiques. Arena reste le défaut ; aucune retouche de ses fonctions de dessin ou des quatre ressources intégrées, aucune animation nouvelle à juger. Pas de nouvelle démo vidéo ; le dernier MP4 de référence demeure V21 (rendu non validé).
- Tests : `node --check` OK ; 11 assertions Playwright ciblées réussies (Arena par défaut, changement dans les trois sens, identité des données hors préréglage, trois rendus distincts à un instant, détection réglage personnalisé, restauration JSON de Sport et absence d’erreur JS). Pas de test de rendu complet vidéo pour Sport/Prestige ni de test réel Samsung ; stockage simulé. Les points graphiques et les contrôles V24 ne sont pas réouverts.
- Suite : FN-06, créer les gabarits spécifiques annonces de tournois, résultats et performances/podiums ; prévoir champs dédiés et réutilisation sans joueur/photo obligatoire, et tests ciblés. Ensuite FN-07 recette sur appareils, FN-08 et OPS-01 selon autorisation. Aucun GO supplémentaire pour le développement indépendant, pas de publication, animations/bande-son reportées.

## 0D. MAJ24 — point de reprise prioritaire

- FN-02 : navigation mobile fixe par cinq rubriques (Aperçu, Projet, Visuel, Cartes, Fichiers), zones tactiles et champs agrandis, boutons flexibles, libellés accessibles pour l’ordre et la suppression, aperçu plus compact. Contrôles Chromium à 320, 360, 412, 768 et 1280 px ; accès direct aux cartes ; reste à vérifier sur Samsung réel.
- FN-04 : écran final activable indépendamment, durée 1,5 / 2,2 (défaut historique) / 3 / 4 / 5 s, logo optionnel, texte principal réellement facultatif, informations compétition/date ou deux lignes personnalisées ou aucune. Aperçu et export PNG dédiés ; sélection finale conservée après réorganisation ; intro seule ne produit pas d’outro. Réglages sauvegardés/restaurés dans JSON v1 avec valeurs historiques par défaut pour anciens projets. Choix d’ergonomie et durées proposés, non validés par utilisateur.
- Tests : `node --check` OK ; 20 assertions ciblées Playwright, toutes réussies, dont comparaison pixel exacte V23/V24 à cinq instants en 720p avec réglages par défaut (intro, cartes, outro), absence de débordement, navigation, durée, aperçu, réorganisation, PNG 3 formats, JSON et absence d’erreur JS. Stockage simulé, pas de test réel Android/iPhone. Le moteur d’animation des joueurs reste inchangé ; pas de nouvelle démo d’animation, pas de recette MP4 native supplémentaire.
- Suite : FN-05 modèles indépendants, puis FN-06 gabarits annonces, résultats et performances. Animations reportées, export natif à valider, pas de publication ni de bande-son. GO acquis.

## 0C. MAJ23 — point de reprise prioritaire

- FN-03 : ajout d'un mode qualité MP4 H.264 déterministe à 30 i/s (WebCodecs VideoEncoder, VideoFrame, timestamps fixes et multiplexage AVC/MP4 local, sans bibliothèque externe ni service payant). Le mode utilise un temps de dessin indépendant du temps réel, vérifie l'ordre, le nombre et la configuration des images, impose une limite mémoire de 240 Mio de données encodées. Le mode secours MediaRecorder reste disponible sur choix explicite, fichier nommé `temps-reel` et cadence non garantie. Annulation, progression, réactivation des contrôles et message d'incompatibilité explicites. Le mode qualité exige un contexte sécurisé et un encodeur AVC compatible ; ne pas promettre la compatibilité Safari/iPhone, Samsung ou fichier HTML local sans test. Aucun changement graphique : chaînes base64 identiques et fonction draw identique à V22.
- Contrôles réels : `node --check` OK. Multiplexeur testé avec 90 échantillons H.264 issus des trois premières secondes de la démo V21 réencodée sans B-frames : ffprobe 720×1280, 30/1 i/s, 90 images, durée 3,000 s ; décodage intégral sans erreur. 8 assertions Playwright réussies : largeur mobile, indisponibilité de VideoEncoder dans le contexte de test, refus explicite et réactivation des contrôles, orchestration des 90 timestamps avec encodeur simulé alimenté par ces échantillons préencodés, réactivation, annulation, export de secours réel, absence d'erreur JS non gérée. Le MP4 produit par l'encodeur simulé n'est PAS un export natif du rendu ; ne pas le présenter comme une nouvelle démo. Le MP4 de secours est bien issu du bouton d'export. La démo V21 reste la référence graphique, animations volontairement reportées et non validées.
- Limites : navigation HTTP bloquée par l'environnement de test (ERR_BLOCKED_BY_ADMINISTRATOR), contexte non sécurisé ; impossible de tester ici la véritable chaîne WebCodecs H.264. FN-03 reste partiel jusqu'à recette native 720/1080 et formats, durée/charge pour 9 joueurs, compatibilité Samsung et iPhone. Ne pas refaire les tests V22 sans motif. Pas de publication, aucune donnée réelle modifiée, aucune bande-son.
- Suite : FN-02 ergonomie mobile, FN-04 écran final, FN-05 modèles interchangeables et FN-06 annonces/résultats. Tester FN-03 sur appareil réel au moment opportun, après préparation d'un contexte HTTPS gratuit autorisé ; pas de sollicitation ni de GO supplémentaire pour avancer sur les chantiers indépendants. Préserver V22 et V23 ; le présent pack inclut les preuves, l'ancien pack et la référence originale sont conservés.

## 0B. MAJ22 — point de reprise prioritaire

- Retour utilisateur sur V21 : « Je ne suis toujours pas fan mais bon on reviendra dessus plus tard. Il faut continuer ». AN-01/02/04/05/06 : finition visuelle reportée sur décision utilisateur, non validée ; conserver la base V21, les choix AN-03 et la référence HIVE. Bande-son toujours reportée. Aucun changement des fonctions de dessin ni des quatre images intégrées. Priorité désormais fonctionnelle.
- FN-01 : source V22 `MILFT_Communication_V22_Arena.html`. Normalisation des noms (Unicode NFC, casse et espaces), import de bibliothèque atomique et non écrasant, protection des données locales illisibles, avertissement explicite si stockage indisponible/plein, suppression indépendante du montage, sélection d'aperçu qui suit la carte réordonnée ou supprimée, chargement photo atomique, contrôle des photos locales et des réglages JSON avant remplacement du montage. Les réglages absents dans les anciens JSON v1 reprennent les valeurs par défaut (choix technique pour éviter la contamination par le projet précédent). Logo officiel rétabli si ancien JSON sans champ logo. Libellé « Scène Arena » plutôt que « Scène 3D » pour décrire le moteur réel.
- Tests réellement effectués : `node --check` OK ; Chromium/Playwright avec injection HTML, viewport mobile 412 px. 20 assertions passées (voir `tests/test22.py`, `tests/test22.log`) : photo, bibliothèque, doublons, import invalide, écriture simulée, ajout/suppression, ordre, ancien JSON, 9 joueurs/8 raccords 39,8 s sans intro/outro, échantillonnage rendu aux frontières, sauvegarde JSON, refus projet invalide, PNG 720×1280 / 720×900 / 720×720, téléchargement export vidéo natif, aucune erreur JS. Navigation HTTP bloquée par l'environnement, `localStorage` remplacé par un objet simulé ; persistance réelle après fermeture, capacité, compatibilité anciens fichiers effectivement utilisés et Android/iPhone restent à vérifier. Le test d'écriture n'est pas une preuve de persistance réelle. Aucun test visuel complet sur 9 joueurs.
- FN-03 : véritable export natif depuis le bouton de l'app, `MILFT37_Arena_V22_Export_Natif.mp4`, 1 carte fictive avec image synthétique bleue, sans intro/outro, 3 s demandées. FFprobe : H.264, 720×1280, 2,938 s, 292253 octets, cadence moyenne 345000/44071 ≈ 7,83 i/s ; avertissement FFmpeg DTS non monotone sur sortie null lors du décodage. Export MP4 réel mais cadence et précision temporelle non conformes à la cible 30 i/s ; ne pas déclarer l'export validé. Pas d'export vidéo 1080 ni Safari/Android réel contrôlé. La démo V21 reste le dernier rendu graphique à 30 i/s ; V22 ne modifie pas ces animations.
- Suite immédiate : FN-03 export fiable et cadence régulière (évaluer encodage déterministe/horodatage par image et solution gratuite compatible mobile, mesurer performance) ; FN-02 ergonomie mobile ; FN-04 outro et FN-05 modèles indépendants puis FN-06. Revenir aux animations seulement après avancée fonctionnelle, sans déclarer le visuel validé. Pas de nouvelle publication ni de GO requis.
- Pack MAJ22 incrémental : V20, V21 et V22, démo V21, export natif V22, référence Instagram, scripts et résultats, présente feuille et manifeste SHA256. Packs historiques MAJ19/20/21 inchangés.

## 0A. MAJ21 — point de reprise prioritaire

- Reprise après conversation en lecture seule : ZIP MAJ20 et MP4 V20 localisés mais extraction binaire refusée ; HTML V20 intégral et feuille MAJ20 récupérés en texte (2 144 316 et 26 957 octets), vidéo Instagram originale récupérée en binaire. Feuille relue, séquence HIVE revue à 2 images/s. Aucun nouveau GO nécessaire.
- Source V21 : `MILFT_Communication_V21_Arena.html`. AN-01 : nouvelle trajectoire avec inclinaison verticale (pitch), approche de biais et accélération/décélération quintique ; logo agrandi en sortie vers le haut ; caméra et éclairage continus. Raccord encore expérimental ; sur les images de contrôle le texte quitte le cadre vers le haut et la scène n’a pas encore le volume HIVE. AN-05 : ondulations amplifiées durant le déroulement, courbure du bord libre et atténuation vers la fixation. Pas de moteur 3D réel ni simulation physique complète ; AN-06 à étudier (WebGL, scène multi-plans / géométrie) en conservant les assets. Ne pas présenter le prototype comme définitif.
- AN-03 : les quatre chaînes d’image base64 sont exactement identiques à V20 ; les réglages et compositions fixes sont conservés. Aucun changement de bande-son, publication ni données réelles.
- AN-02 : démo de trois joueurs fictifs (même portrait, noms distincts, numéro facultatif au troisième), deux raccords de 1,6 s. Caméra et éclairages sur horloge commune. Vérification visuelle par échantillonnage des images décodées ; avis utilisateur encore nécessaire pour conclure à la fluidité. 
- Contrôles effectivement effectués : `node --check` OK, Chromium/Playwright avec injection HTML, chargement des assets OK, rendu déterministe de 621 images JPEG encodées H.264 par FFmpeg. `ffprobe` : 720×1280, 30 i/s, 20,7 s, 5 015 216 octets ; décodage intégral FFmpeg sans erreur. Tests de rendu à plusieurs instants dont frontières dans 9:16 (720×1280), 4:5 (720×900) et 1:1 (720×720), puis sans intro (15,2 s) : aucune exception JS. Pas d’export MP4 natif MediaRecorder testé, pas de recette fonctionnelle complète, ni test Samsung/iPhone/Windows. Démo externe au mécanisme d’export de l’application.
- Livrables : HTML V21, MP4 V21, feuille MAJ21, pack de reprise incrémental avec HTML V20 récupéré, référence Instagram et scripts de génération/contrôle. Le ZIP historique MAJ19/20 demeure inchangé et n’est pas remplacé intégralement. Les quatre assets nécessaires au rendu sont intégrés dans les HTML.
- Suite : AN-06 prototype comparatif ciblé véritable 3D ou multi-plans, prioriser raccord logo→scène et lumière/tissu. AN-02 valider fluidité avec le MP4 V21 puis endurance 8–9 joueurs ; FN-01 et FN-03 poursuivre les tests indépendants. Ne pas refaire les validations AN-03. Aucun GO technique supplémentaire ni publication ; aucune manipulation requise maintenant.

## 0. Mise à jour MAJ20 — point de reprise prioritaire

- Source actuelle : `MILFT_Communication_V20_Arena.html`. Démo : `MILFT37_Arena_V20_Demo.mp4` (H.264, 720 × 1280, 30 i/s, 453 images, 15,1 s, sans son ; deux joueurs fictifs, durée carte 4 s, intervalle 1,6 s, pas d’outro).
- Reprise : pack MAJ19 localisé dans la bibliothèque mais extraction binaire du ZIP et du MP4 V19 refusée par l'environnement. Feuille MAJ19 relue intégralement, source V19 complète récupérée sous forme de texte HTML, source Instagram originale récupérée et examinée autour de 3 s. Les sections 1–10 ci-dessous décrivent l'historique MAJ19 ; le présent bloc prévaut pour la reprise.
- AN-01 : nouvelle trajectoire de caméra et sortie progressive du logo vers le haut ; découverte du décor de biais puis approche continue. Suppression du passage par le montant de V18/V19. Correction du dessin parasite du fond dans `bannerScene(textureOnly=true)` qui annulait l'opacité au début du raccord. Rendu Canvas 2D toujours, pas de vraie scène 3D. Raccord non validé par l'utilisateur.
- AN-02 : horloge unique pour caméra et éclairages, y compris lors du changement de joueur. Suppression de la rupture de trajectoire au premier changement ; durée et principe remontée/déroulement V19 conservés. Démo à deux joueurs uniquement.
- AN-05 : plis plus progressifs, combinaison de deux ondes, ourlet qui se courbe au déroulement ; intensité des faisceaux réduite. Réalisme physique à améliorer et à juger par l'utilisateur.
- AN-03 : les quatre données d'image intégrées sont identiques à celles du HTML V19 récupéré (comparaison exacte des chaînes base64). Logo, décor, photo et bâche préservés ; métal 12 %, acier et rails désactivés conservés. Titre, en-tête et pied de page alignés V0.20.
- Tests : `node --check` OK. Chromium exécuté par Playwright avec injection du HTML dans une page vide (navigation locale bloquée). Assets chargés, démo dessinée à pas de temps déterministe et encodée avec FFmpeg. Vérification ffprobe du fichier final ; images autour des raccords examinées. Le début a été recalculé après la correction du fond ; la fin provient du rendu V20 précédent, identique sur le plan de la composition lorsque l'opacité de scène vaut 1. Pas de test de l’export MediaRecorder de l'application, pas de recette Samsung/iPhone, pas de comparaison directe avec le MP4 V19 faute de fichier binaire accessible.
- Prochaine MAJ : AN-01/AN-05, renforcer le lien spatial logo-scène, évaluer une approche 3D si le Canvas plafonne ; AN-02 vérifier plusieurs joueurs. Puis poursuivre les points indépendants de la feuille de route. Aucun GO supplémentaire nécessaire pour le développement ; arbitrage visuel de la démo V20 utile. Ne pas traiter le son ni publier.
- Pack MAJ20 incrémental : contient la feuille complète, HTML V20, MP4 V20, référence Instagram et HTML V19 récupéré. Le pack historique MAJ19 reste inchangé dans la bibliothèque, et contient les autres assets et versions anciennes. Le nouveau pack ne prétend pas remplacer l'archive historique intégrale.

## 1. Résumé opérationnel / point de reprise (historique MAJ19)

- Dernière version : `MILFT_Communication_V19_Arena.html`.
- Dernière démonstration : `MILFT37_Arena_V19_Demo.mp4` (2 cartes fictives, même portrait). Vérifiée le 25/11 : H.264, 720 × 1280, 30 images/s, 15,1 s. Le code JavaScript passe `node --check`. Aucun nouveau test fonctionnel complet du navigateur effectué lors de la rédaction de cette MAJ.
- Retour utilisateur après la démonstration V0.19 : « Ok ». Accord pour poursuivre, pas une validation de mise en production ni de tous les parcours de l'application. L'enchaînement des joueurs est accepté comme première base.
- **Prochaine MAJ = V0.20** : améliorer en priorité la transition logo → scène, toujours jugée perfectible en V0.18 ; consolider la continuité entre joueurs. Ne pas recommencer le graphisme validé.
- **Aucune action utilisateur indispensable pour poursuivre le développement graphique.** Une photo réelle et un test Samsung seront nécessaires plus tard, pas maintenant.
- Bande-son expressément reportée. Aucun achat, abonnement, hébergement payant ou publication automatique sans accord.

## 2. Cahier des charges

Application MILFT Communication, distincte de MILFT Tournois et MILFT Compta, permettant aux responsables du club de fabriquer facilement et à répétition des publications Facebook et Instagram, sans refaire un montage manuel.

### Périmètre fonctionnel

- Intro logo seule ; présentation d'un joueur ; présentation d'une équipe (ordre et nombre libres) ; félicitations, podiums, performances, qualifications ; annonces de tournois ; résultats ; communication libre.
- Bibliothèque de joueurs : identité, photo, cadrage ; rôle, numéro, résultat et compétition sont des données propres au montage et non des attributs permanents.
- Modèles graphiques indépendants du contenu : changer de modèle sans ressaisir les joueurs. Plusieurs styles à terme (Arena, compétition, prestige, événement, institutionnel, festif ; noms et styles hors Arena = propositions à valider).
- Prévisualisation animée, export MP4 sans bande-son pour l'instant ; PNG fixe ; formats 9:16, 4:5, 1:1 ; résolution 1080 px ou 720 px selon besoin.
- Sauvegarde/restauration des projets et de la bibliothèque ; réutilisation d'une session à l'autre ; objectif gratuit, Android prioritaire (Samsung Galaxy S25 Ultra), puis Windows et iPhone/Safari.
- Pas de dépendance obligatoire à un service payant. Le partage et la sauvegarde Drive automatiques ne sont pas implémentés et restent à décider. Les JSON peuvent déjà être conservés manuellement sur Drive.

## 3. Décisions visuelles à protéger

| Élément | Décision utilisateur / règle |
|---|---|
| Logo | Le fichier `37497.png` est la source officielle. Garder intact. Version communication : `MILFT37_Logo_Communication.png` (PNG transparent, recadrée, sans la petite goutte bleue isolée en bas à droite). Ne pas la réintroduire ; ne pas redessiner le logo. |
| Palette | Bleu dominant, électrique et nuit ; rouge et jaune du logo conservés. Personnalisation possible. |
| Relief du logo | Base esthétique V0.5 Polished Metal approuvée (« C'est vachement mieux »). Épaisseur par défaut 12 %, réglable 5–35 %. Acier/chrome poli ou or poli ; reflets mobiles, arêtes lumineuses fines ; ni strates multicolores, ni plastique mat, ni épaisseur 24 % par défaut. |
| Intro | Plusieurs mouvements, ralentissement au passage de face, présence suffisante du logo, pas de retour artificiel ni de saccades. V0.12 jugée meilleure, mais une gêne résiduelle non identifiée demeure : ne pas déclarer l'animation définitive. |
| Traits latéraux intro | Suppression validée après V0.17 (« Ok pour les traits ») ; désactivés par défaut. Ne pas confondre avec les tubes d'éclairage de la scène joueur. |
| Présentation Arena | Grande bâche bleue réellement suspendue à une structure de scène, portrait imprimé sur le tissu, nom sur une ligne si possible, rôle et compétition lisibles, pas de gros logo au-dessus, pas de répétition « Montlouis Football de Table ». Logo sur le polo seulement lorsque présent sur la photo. |
| Référence de composition | `1795556588788.png` = affiche source avec bâche (à ne pas réinterpréter). `a_highly_detailed_realistic_promotional_poster_si.png` = référence visuelle corrigée, sans gros logo supérieur et avec baby-foot flouté ; approuvée par « Ok » après demande de flou. |
| Baby-foot | Bonzini B90 ITSF (photo fournie `35429.jpg`). Gros plan au ras du terrain, barres et figurines rouges/bleues, légèrement flouté au premier plan ; doit rester secondaire. Pas de table entière, pas de caisse imposante, pas de publicité ni de marquages inventés. |
| Texte / rôle | Rôle facultatif et libre (capitaine, coach, remplaçant, etc.) ; aucun bandeau par défaut pour les autres joueurs si aucune mention utile. Réorganiser les textes sans laisser de trou. Numéro facultatif, distinct du rôle, dépend de la compétition. Résultat facultatif. |
| Photo | Portrait fictif seulement pour les tests (ne pas publier comme un vrai joueur). Remplacer par de vraies photos autorisées plus tard, préserver les personnes et leurs vêtements. |
| Son | Reporté par l'utilisateur. Ne pas développer maintenant. |

**Interdits de reprise :** ne pas substituer une autre affiche à la bâche approuvée ; ne pas régénérer intégralement un visuel pour une retouche locale ; ne pas remplacer le logo officiel par une approximation IA ; ne pas ajouter un N°1 systématique ; ne pas transformer le baby-foot en sujet principal.

## 4. Animation de référence et problèmes ouverts

Source originale : `Screen_Recording_20261124_211019_Instagram.mp4` (10,855 s ; capture verticale 720 × 1560). Publication : https://www.instagram.com/p/DgH9nidiCHn/?jplx=ZGs2azZwbjhhZHo1 . Travailler sur le fichier local ; la publication peut être inaccessible. L'extrait comporte l'interface Instagram ; ne pas l'intégrer au résultat.

- Avant ~3 s : logo métallique en rotation, révélation d'une structure de scène. Revoir les images de la source pour la trajectoire exacte plutôt que d'inventer une transformation. Les temps sont indicatifs et non un relevé de montage définitif.
- À partir de ~3 s : séquence particulièrement importante demandée par l'utilisateur. Caméra en mouvement continu, déroulement de la bâche, plis et ondulations, ombres et effets de lumière sur tissu et décor. Le portrait est mis en valeur, sans perdre sa lisibilité.
- Le joueur doit rester intégré à une scène vivante ; pas de pause fixe en arrivant de face puis de reprise brutale, pas de zoom/dézoom artificiel, pas de mouvements bizarres du portrait seul, pas de flash aveuglant.
- V0.15 : fluidité de la présentation joueur améliorée et jugée meilleure. V0.16 : transition jugée « bof ». V0.18 : passage derrière un montant métallique, jugé « Mieux mais pas encore top ». **Transition logo → joueur NON VALIDÉE.**
- V0.19 : nouvelle transition interjoueurs, 1,6 s, première bâche remonte et seconde se déroule dans le même décor ; caméra et éclairages maintenus ; pas de nouvelle intro. Retour « Ok » : base à conserver pour les prochaines itérations.
- La simulation actuelle est Canvas 2D avec projection en perspective, et non un véritable moteur de rendu 3D réaliste. Ne pas confondre un MP4 à 30 i/s avec un mouvement visuellement fluide.

## 5. Historique des versions

| MAJ | Évolution | Statut / retour utilisateur |
|---|---|---|
| 01 | Prototype paramétrable (logo, photos, textes, formats, projets, aperçu, export) | Base technique |
| 02 | Arena Blue, intro logo | Goutte bleue décentre le logo |
| 03 | Logo communication sans goutte, épaisseur portée à 24 % | Trop de strates |
| 04 | Tranche acier et or uniforme | Trop épais ; manque de brillance |
| 05 | 12 %, reflets polis animés, rails optionnels | Rendu métal approuvé |
| 06 | Player Reveal, cartes multiples, transitions et cadrage | Base technique |
| 07 | Grande bâche Arena, rôle et numéro optionnels, décor et portrait séparés | Graphisme de référence approuvé ; implémentation à affiner |
| 08 | Animation tissu, variantes de révélation, export PNG | Intégré ; essais Chromium annoncés |
| 09 | Bibliothèque joueurs et JSON | Intégré ; essais Chromium annoncés |
| 10 | Transition caméra vers scène, rotation lissée | Rejet graphique de la transition |
| 11 | Structure projetée en volume | Expérimental, logo à peine visible |
| 12 | Intro prolongée, ralentissements, zoom et lumières joueur | Mieux, gêne résiduelle non identifiée |
| 13 | Effets joueur accentués | À rapprocher davantage de HIVE |
| 14 | Déroulement, plis et mouvements accentués | Rejet : arrêt sur joueur puis mouvements artificiels |
| 15 | Trajectoire continue, suppression du changement de rendu sur arrivée joueur | Mieux ; manque de transition |
| 16 | Transition intermédiaire logo/structure | « Bof » |
| 17 | Traits lumineux intro désactivés | Suppression validée, transition non validée |
| 18 | Passage derrière montant, découverte de biais | Mieux, mais transition pas encore au niveau |
| 19 | Changement de bâche entre deux joueurs | « Ok » ; version de reprise, non production |

## 6. État technique actuel, vérification et limites

L'application V0.19 est un fichier HTML autonome (CSS/JavaScript, Canvas 2D) ; logo, décor, bâche et portrait de démonstration intégrés. `draw()` gère l'enchaînement ; `draw18()` la première présentation et le raccord ; `arenaWorld11()` la scène projetée ; `turnLogo11()` la rotation du logo ; `postPass18()` le passage derrière le montant ; `teamGap19()` fixe l'intervalle interjoueurs à 1,6 s dans le modèle bâche/scène. `total()` et `refresh()` gèrent la durée et l'aperçu.

| Fonction | État | Contrôle / réserve |
|---|---|---|
| Intro autonome, acier/or, épaisseur et rails | Implémenté ; esthétique partiellement validée | Préserver V0.5 et V0.17 ; rotation V0.12 non définitive |
| Présentation Arena, nom/rôle/numéro/résultat et photo | Implémenté | Affiche validée ; vérifier fidélité de toutes les cartes générées |
| Multi-joueurs, ordre, bibliothèque | Implémenté dans le code | Tests Chromium annoncés antérieurement ; endurance, 8–9 joueurs et données réelles à vérifier |
| Sauvegarde projet JSON, import/export bibliothèque | Implémenté | Stockage navigateur `localStorage` (`milft-com-library-v1`) ; capacité et persistance réelles à vérifier |
| Export vidéo | Implémenté | `captureStream(30)` + `MediaRecorder`, MP4 si supporté sinon WebM ; export mobile et cadence réelle non garantis |
| Export PNG | Implémenté | Bouton export carte ; vérifier capture de la bonne carte sans mouvement parasite |
| Résolutions / formats | Implémenté | Vérifier toutes les compositions et exports 9:16, 4:5 et 1:1 ; démo V19 en 720p, pas une validation Full HD |
| Annonces, résultats, communication libre | Options présentes | Parcours et gabarits spécifiques à finaliser, pas validés |
| Choix d'ambiances / cartes | Options présentes | Véritable bibliothèque modulaire de modèles indépendants à développer |
| Android / iPhone / Windows | À valider | Aucun test Samsung/iPhone réel consigné ; Chromium testé selon les comptes rendus précédents |
| Drive / partage | Non développé | Export JSON manuel seulement ; pas de synchronisation ni publication automatique |
| GitHub / production | Non mis en place à ce stade | Aucun dépôt, URL de production ou workflow CI confirmé dans cette session |

### Contrôles effectués à la rédaction MAJ19

- Les fichiers V01 à V19 sont présents dans le dossier de travail. Syntaxe JS V19 vérifiée avec Node, sans erreur.
- Démo V19 contrôlée avec ffprobe : 720 × 1280, H.264, 30/1 i/s, 15,1 s. V17/V18 : 720 × 1280, 30 i/s, 9,5 s chacune.
- La durée du montage dans l'app dépend des options : intro scène 5,5 s, cartes 3/4/5/7 s, intervalle 1,6 s, écran final optionnel 2,2 s. Ne pas assimiler les paramètres de la démonstration aux réglages par défaut.
- Petite incohérence de version constatée : en-tête V0.19 mais pied de page V0.18 et titre navigateur « Prototype ». À harmoniser lors d'une prochaine MAJ, sans toucher à la base archivée.
- Vérification des médias source : logo officiel 1414 × 2000 RGBA, zone utile 544 × 517 ; version communication 519 × 517 RGBA. La version HD est un agrandissement interpolé, non vectoriel.
- Les affirmations de tests des versions précédentes sont conservées comme historique ; elles ne valent pas une nouvelle recette V19 exécutée. Aucun test nouveau sur appareil réel ni déploiement pendant cette MAJ documentaire.

## 7. Feuille de route priorisée (à mettre à jour à chaque version)

Légende : **V** validé utilisateur sur le point précis ; **I** implémenté, recette à consolider ; **E** expérimental ; **A** à faire ; **R** reporté.

| ID | Priorité | Action / livrable | État | Critère de clôture |
|---|---|---|---|---|
| AN-01 | Reporté | Transition intro logo → scène | E, non validé | MP4 comparé à HIVE ; raccord naturel, trajectoire continue, aucun fondu incohérent ou arrêt ; retour utilisateur positif |
| AN-02 | Reporté | Fluidité de la présentation et de l'enchaînement interjoueurs | I, non validé visuellement | Préserver V15/V19 ; vérifier continuité position, vitesse, lumière et tissu aux frontières, 2 puis plusieurs joueurs |
| AN-03 | P0 | Intro sans rails, métal poli, logo sans goutte | V pour ces choix | Pas de régression ; ne pas refaire les choix validés |
| AN-04 | Reporté | Gêne résiduelle de l'intro | E | Comparaison A/B ciblée en MP4 ; durée et lisibilité des faces, rythme et fin de rotation ; pas d'altération du logo |
| AN-05 | Reporté | Fidélité physique de la bâche et lumières | E | Mouvement visible mais naturel, portrait lisible, même décor et baby-foot flou ; texture/plis continus |
| AN-06 | P1 | Étudier alternative véritable 3D (ex. WebGL ou rendu Blender) si la simulation plafonne | R (reporté après retour V21) | Prototype comparatif, ressources libres/gratuites, compatibilité mobile et réutilisation des textes/photos ; pas de migration aveugle |
| FN-01 | P1 | Recette bibliothèque et projets (ajout, doublons, suppression, ordre, sauvegarde/restauration, anciens JSON) | I, tests ciblés V22 OK (stockage simulé) | Tests synthétiques non destructifs ; contrôle des données avant/après |
| FN-02 | P1 | Ergonomie sur écran Samsung ; navigation, cadrage, aperçu et export | I, contrôles V24 | Interface lisible, sans défilements excessifs ; test Chromium mobile puis test réel lorsque indispensable |
| FN-03 | P0 fonctionnel | Export MP4 fiable et formats sociaux | I, MP4 natif obtenu mais cadence insuffisante | 1080×1920 / 1080×1350 / 1080×1080, option 720 ; contrôle durée, codec, image finale et lecture. Ne pas présenter WebM comme MP4 |
| FN-04 | P1 | Clôture/outro optionnelle et réutilisable | I, contrôles V24 | Cohérence avec l'intro, durée, texte facultatif ; pas de logo supplémentaire sur les fiches |
| FN-05 | P2 | Architecture de modèles graphiques réutilisables | I, préréglages V25 | Contenu séparé du rendu, switch sans perte ; Arena puis nouvelles déclinaisons |
| FN-06 | P2 | Gabarits performances/podiums, annonces et résultats | I, contrôles V26 | Champs spécifiques, couleur/style et badge facultatifs, cas réels de club |
| FN-07 | P2 | Recette Windows, Android, Safari iPhone | A | Import photo, sauvegarde, restauration, PNG/vidéo et lecture locale ; énoncer limites par navigateur |
| FN-08 | P2 | Stratégie de stockage photos et données / Drive | I, sauvegarde manuelle V27 | Aucun coût, sauvegarde manuelle fiable ; décider ultérieurement partage/synchro avec autorisation |
| OPS-01 | P2 | Dépôt dédié, versionnement, tests automatiques et hébergement gratuit | A | Dépôt distinct si autorisé, pas de modification des dépôts Tournois/Compta ; feuille de route et assets documentés ; workflow de validation |
| OPS-02 | P2 | Recette finale et publication | A | Validation utilisateur sur appareil réel et GO explicite avant publication ; conserver versions précédentes |
| SND-01 | Hors priorité | Bande-son et choix de sons libres/droits | R | Reprendre seulement après accord utilisateur |

### Ordre de reprise immédiat

1. Ouvrir V19 et revoir **la vidéo source HIVE**, notamment la séquence autour de 3 s, puis comparer aux démos V18 et V19.
2. Créer V20 dans un nouveau fichier. Isoler d'abord le raccord logo-scène ; ne pas modifier la composition validée ni le changement de bâche V19. Tester une trajectoire et une occlusion physiquement cohérentes, avec continuité de vitesse ; si la technique ne permet pas le rendu, l'indiquer et proposer une comparaison 3D ciblée plutôt que des variantes quasi identiques.
3. Produire un vrai MP4 jouable (pas de GIF, planche ou aperçu statique comme substitut). Contrôler les images autour des raccords et le fichier vidéo, puis livrer le HTML correspondant. Tester sans son, avec deux joueurs fictifs et le même contenu pour isoler les différences.
4. Poursuivre sur les tâches indépendantes sans attendre un GO systématique : vérification de la bibliothèque, cas à plusieurs joueurs, formats, ergonomie. Ne pas réouvrir les décisions graphiques validées sans demande. Solliciter l'utilisateur pour un arbitrage visuel substantiel ou un test réellement impossible à simuler.

## 8. Protocole de travail autonome (à respecter dans chaque chat)

- Considérer le GO pour le développement courant acquis. Travailler directement sur la dernière source vérifiée et avancer dans le tour courant tant que les outils le permettent. Ne pas réclamer de GO entre deux micro-étapes. Ne pas promettre de travail en arrière-plan.
- Lire cette feuille et les fichiers de référence avant toute modification. Vérifier que la version de départ est bien la dernière ; si un nouveau fichier plus récent existe, le comparer et réconcilier la feuille. Ne pas repartir d'une ancienne version par erreur.
- Une MAJ = nouveau fichier versionné ; conserver l'ancien intact. Ne jamais écraser les sauvegardes/projets/photos réels ni les données de Tournois/Compta. Tester sur données fictives isolées. Aucun envoi de données ou publication sans autorisation.
- Garder le code, les médias et le document de reprise alignés. Les visuels validés sont des références fixes ; faire des modifications localisées. Éviter les générations d'images quand le besoin est de corriger une animation ou un export paramétrable.
- Vérifier autant que possible de manière autonome : syntaxe JS, exécution navigateur, absence d'erreurs console, tests ciblés, export réel, inspection du MP4, régression des réglages. Préciser l'environnement, le résultat et les limites. Ne pas annoncer un test qui n'a pas été réellement exécuté.
- Distinguer : **implémenté**, **testé techniquement**, **validé visuellement par l'utilisateur**, **testé en réel sur mobile**, **publié**. Un « mieux » n'est pas un feu vert production. Ne pas retester systématiquement les points validés, sauf risque de régression.
- Ne solliciter l'utilisateur que si une décision visuelle importante, l'accès à un service, une photo réelle ou un test appareil l'exige. Si intervention, expliquer exactement quoi faire, sur Samsung en priorité. Sinon, poursuivre les tâches indépendantes.
- À chaque avancée significative : numéro MAJ, fichier/commit si dépôt créé, modifications, preuves de tests, retour utilisateur exact, problèmes non résolus, prochaines tâches, intervention utilisateur requise (oui/non). Maintenir cette feuille et fournir une version actualisée à la fin de la session.
- Changement de chat : joindre le pack actualisé ; ne jamais présumer qu'un lien sandbox ancien reste accessible. À terme, un dépôt GitHub dédié pourrait servir de source de vérité durable, mais aucun dépôt n'est créé par cette MAJ.

## 9. Fichiers de reprise

Le ZIP associé contient une copie de ce document, les sources HTML historiques disponibles, les ressources utiles, les vidéos de référence et les démonstrations clés. Les fichiers sont archivés sans modification ; le manifeste SHA-256 permet de vérifier leur intégrité.

| Chemin dans le pack | Utilité |
|---|---|
| `sources/MILFT_Communication_V19_Arena.html` | Dernière source ; base pour V20 |
| `sources/` | Versions antérieures, historique et retour arrière |
| `demos/MILFT37_Arena_V19_Demo.mp4` | Dernière vidéo à deux joueurs |
| `demos/` | Références V05 acier/or, V12, V15, V17, V18 ; comparaison des corrections |
| `references/Screen_Recording_20261124_211019_Instagram.mp4` | Source HIVE originale, essentielle pour les transitions |
| `references/1795556588788.png` | Affiche originale avec bâche |
| `references/a_highly_detailed_realistic_promotional_poster_si.png` | Affiche corrigée approuvée avec baby-foot flou |
| `references/35429.jpg` | Photo Bonzini B90 ITSF fournie |
| `assets/37497.png` | Logo officiel source intact |
| `assets/MILFT37_Logo_Communication.png` | Logo sans goutte pour les communications |
| `assets/MILFT37_Logo_HD_transparent.png` et `MILFT37_Logo_original_recadre.png` | Recadrages avant suppression de la goutte ; archives, non logo par défaut |
| `assets/Arena_V07_Decor.jpg`, `Arena_V07_Bache_vide.jpg`, `Arena_V07_Portrait_demo.png` | Ressources séparées du rendu actuel |
| `SHA256SUMS.txt` | Empreintes des fichiers du pack (hors manifeste) |

## 10. Message prêt à copier dans un nouveau chat

> Reprends le développement de MILFT Communication après la MAJ 19. GO déjà donné. Lis en priorité la feuille de route du pack joint et utilise la V0.19 comme base de reprise. Respecte le protocole de travail autonome comme pour MILFT Tournois : ne me sollicite que si indispensable, ne refais pas les validations acquises, conserve les versions et mets à jour la feuille de route après chaque avancée. Revois la vidéo Instagram HIVE incluse, en particulier à partir de la troisième seconde. Priorité V0.20 : rendre naturelle la transition logo → scène en conservant le graphisme validé et la transition entre joueurs ; fournir une vraie démonstration MP4, pas une planche d'images. Ne remets pas la goutte bleue ni les traits latéraux de l'intro ; pas de bande-son pour l'instant. Travaille sur données fictives, sans toucher à MILFT Tournois/Compta ni publier. Continue ensuite les points indépendants de la feuille de route sans attendre de nouveaux GO.

## 11. Journal de reprise (à compléter)

| MAJ | Date | Action et preuve | Statut / retour | Suite | Intervention |
|---|---|---|---|---|---|
| 19 | 25/11/2026 | Consolidation documentaire ; syntaxe V19 OK, MP4 vérifié par ffprobe ; pack de reprise | V19 base de travail ; transition intro-scène à améliorer ; aucune production | V20 AN-01, AN-02 | Non à ce stade |

Pour les prochaines lignes, noter les tests réellement réalisés, les chemins des livrables, les réserves et l'état des tâches correspondantes. Ne pas transformer les améliorations proposées en fonctionnalités validées sans preuve.
| 20 | 25/11/2026 | Raccord travelling, caméra continue entre joueurs, tissu et éclairage affinés, bug fond corrigé. Syntaxe JS OK ; MP4 H.264 453 images à 30 i/s, 15,1 s | Prototype V20 à juger visuellement ; 2 joueurs fictifs ; pas de recette réelle | AN-01/02/05 puis tests indépendants | Pas de GO technique requis |
| 21 | 25/11/2026 | Inclinaison caméra, raccord quintique, tissu ; trois joueurs, 621 images H.264 ; tests 3 formats et sans intro sans erreur JS | Prototype à juger, pas de 3D réelle ni export natif validé | AN-06, AN-01/05 puis FN-01/03 | Pas de GO technique requis |

## Message de reprise actualisé MAJ21

> Reprends MILFT Communication après MAJ21, GO acquis. Lis le bloc 0A puis toute la feuille, ouvre le HTML V21 et la référence Instagram du pack. Conserve les graphismes validés, ne recommence pas leurs validations. Priorité : AN-06 prototype comparatif 3D ou multi-plans, AN-01/05 raccord et tissu ; poursuis les vérifications indépendantes. Fournis une véritable vidéo MP4, sans son. Aucune publication. Mets à jour cette feuille après chaque avancée et ne demande mon intervention que si indispensable.


| 22 | 25/11/2026 | Bibliothèque/projets durcis ; 20 contrôles ciblés, PNG 3 formats, MP4 natif H.264 720p | Animation reportée non validée, stockage simulé, MP4 cadence ≈ 7,83 i/s | FN-03 cadence/export puis FN-02/04/05 | Non |

## Message de reprise actualisé MAJ22 (prévaut sur les précédents)

> Reprends MILFT Communication après MAJ22, GO acquis. Lis le bloc 0B et l'intégralité de la feuille. Utilise le HTML V22. Les animations V21 ne plaisent pas encore à l'utilisateur mais leur finition est volontairement reportée ; conserve les graphismes et avance sur les fonctionnalités. Priorité FN-03 fiabiliser l'export vidéo réel et sa cadence, puis ergonomie mobile, outro et modèles indépendants. Ne recommence pas les tests acquis sauf risque de régression. Aucun son, aucune publication, aucune intervention utilisateur sauf nécessité. Mets à jour la feuille et conserve les anciennes versions. Toute nouvelle animation à juger doit être fournie en MP4 réel.


| 23 | 25/11/2026 | Export qualité WebCodecs, MP4 déterministe, 8 contrôles, 90 échantillons H.264 remultiplexés sans erreur | Partiel : encodeur simulé dans le navigateur, secours réel ; test natif à venir | FN-02/04/05/06 et recette FN-03 | Non pour les chantiers indépendants |

## Message de reprise MAJ23 — prévaut

> Reprends MILFT Communication à la MAJ23, GO acquis. Lis le bloc 0C et toute la feuille. Utilise V23. Les animations sont reportées et non validées, graphismes à préserver. Export 30 i/s implémenté, multiplexage et orchestration contrôlés, WebCodecs natif non vérifié ; prévoir recette sur environnement sécurisé et appareils réels, ne pas confondre test simulé et validation. Avancer sans attendre sur ergonomie mobile, écran final personnalisable, modèles graphiques interchangeables, annonces et résultats. Pas de son, pas de publication, pas de modification des données réelles. Consigner les preuves et limites dans la feuille après chaque avancée.


| 24 | 25/11/2026 | Navigation mobile, outro personnalisable et export PNG dédié ; 20 contrôles réussis | Test réel mobile restant, animations inchangées | FN-05/06 | Non |

## Message de reprise MAJ24 — prévaut

> Reprends après MAJ24, GO acquis. Lis toute la feuille et utilise V24. Poursuis les modèles graphiques indépendants et les gabarits annonces/résultats, sans refaire les validations acquises. Animations et bande-son reportées. Pas de publication sans accord explicite.


| 25 | 25/11/2026 | Registre de trois modèles et changement sans perte de contenu, 11 contrôles ciblés OK | Sport et Prestige proposés, non validés ; modèles personnalisés à approfondir | FN-06 | Non |

## Message de reprise MAJ25 — prévaut

> Reprends MILFT Communication après MAJ25, GO déjà acquis. Lis le bloc 0E puis toute la feuille, pars du HTML V25. Priorité FN-06 : annonces, résultats, performances et podiums, sans imposer de photo ou de joueur. Conserve la base Arena et les choix graphiques validés. Ne recommence pas les contrôles acquis sans motif. Les animations sont non validées et reportées, bande-son reportée, aucune publication sans accord. Poursuis les chantiers indépendants, actualise la feuille, conserve les sources.


| 26 | 25/11/2026 | Quatre gabarits sans photo, 18 contrôles ciblés, PNG trois formats | Propositions graphiques, pas de test réel | FN-08 puis FN-07/OPS-01 | Non |

## Reprise MAJ26 — prévaut

> GO acquis. Partir du HTML V26 et lire la feuille complète. Poursuivre FN-08 et préparer FN-07 ; aucune publication ni dépôt externe sans autorisation. Graphismes validés conservés, animations et son reportés.


| 27 | 25/11/2026 | Sauvegarde complète, confirmation, fusion sans écrasement, 10 contrôles ciblés | Stockage simulé, Drive manuel uniquement | Préparer recette FN-07/FN-03 | Non |

## Reprise MAJ27 — prévaut

> GO acquis. Partir du HTML V27 et lire la feuille complète. Poursuivre diagnostic de compatibilité et préparation des tests réels FN-07/FN-03, puis OPS-01 selon autorisation. Aucun dépôt, aucune publication et aucune modification réelle sans accord. Graphismes conservés, animations non validées et bande-son reportées.


| 28 | 25/11/2026 | Diagnostic local, rapport JSON, 10 assertions ciblées, dossier statique et recette groupée | Tests simulés de stockage ; encodeur natif et appareils réels non validés | HTTPS puis recette réelle groupée | Aucun GO intermédiaire ; accord requis avant publication |

## Reprise MAJ28 — prévaut

> Partir de V28, lire toute la feuille. GO développement acquis ; regrouper les chantiers, ne solliciter l’utilisateur que pour un test réel ou une autorisation externe indispensable. Pas de publication ni de modification de données réelles. Finition animation et bande-son reportées.


| 29 | 25/11/2026 | Test MP4 court partagé, annulation, délais anti-blocage, 10 contrôles ciblés, dossier CI préparé | Échantillons préencodés, pas de codec natif ni stockage réel validés, CI non exécutée sur GitHub | Autorisation hébergement de validation puis recette Samsung | Autorisation spécifique nécessaire, pas de GO développement |

## Reprise MAJ29 — prévaut

> Partir du HTML V29 et lire la feuille. GO développement acquis. Hébergement de validation distinct uniquement après accord explicite ; aucun dépôt externe ni publication sans cet accord. Recette groupée Samsung, Windows, iPhone ; conserver graphismes, ne pas rouvrir animation et son.