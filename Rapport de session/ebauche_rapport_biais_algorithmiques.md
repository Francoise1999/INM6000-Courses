# Biais algorithmiques dans la reconnaissance faciale : une technologie discriminatoire peut-elle être éthiquement acceptable ?

---

## Identification

- Djeukam Tchouyomgou Celestine — DJEC12338708
- Marie Françoise Esther E Mentor — MENM04609905
- Soh Mbah Jorex — SOHJ08339707

Cours : INM6000 — Informatique et société
Session : Été 2026
Institution : Université du Québec à Montréal (UQAM)

---

## Titre

**Biais algorithmiques dans la reconnaissance faciale : une technologie discriminatoire peut-elle être éthiquement acceptable ?**

---

## Sujet

La reconnaissance faciale est devenue omniprésente dans les sociétés contemporaines. Des aéroports aux stations de métro, en passant par les commerces, les applications mobiles et les forces de l'ordre, cette technologie promet de simplifier l'identification des individus et d'améliorer la sécurité publique. Selon le rapport du NIST (2019), des centaines de systèmes de reconnaissance faciale sont déployés à travers le monde, utilisés par les gouvernements et les entreprises pour des usages aussi variés que le contrôle frontalier, la surveillance de masse et la vérification d'identité bancaire. Pourtant, derrière cette promesse d'efficacité se cache une réalité beaucoup plus problématique : les algorithmes qui alimentent la reconnaissance faciale ne sont pas neutres. Ils héritent des biais présents dans les données qui servent à les entraîner, et lorsque ces données sous-représentent certaines catégories de la population — notamment les femmes à peau foncée — les conséquences peuvent être graves, allant de simples erreurs de classification à des arrestations injustifiées (Buolamwini et Gebru, 2018).

Ce projet s'inscrit dans le prolongement des travaux de Joy Buolamwini et Timnit Gebru, dont l'étude Gender Shades (2018) a démontré que les systèmes de reconnaissance faciale commerciaux présentaient des taux d'erreur allant jusqu'à 34,7 % pour les femmes à peau foncée, contre moins de 1 % pour les hommes à peau claire. Ces disparités ne sont pas de simples défauts techniques : elles traduisent des inégalités structurelles qui se trouvent amplifiées et institutionnalisées par la technologie. Les travaux du NIST (Grother et al., 2019) confirment cette tendance à une échelle beaucoup plus large, en testant près de 200 algorithmes et en constatant des écarts de précision pouvant atteindre un facteur 7 000 entre les groupes démographiques. En examinant les cas documentés de Robert Williams (Détroit, 2020) et de Michael Oliver (Michigan, 2023), tous deux arrêtés à tort sur la base d'erreurs de reconnaissance faciale, ce projet montre que les biais algorithmiques ne sont pas un problème abstrait mais une réalité qui affecte concrètement les droits fondamentaux des personnes racisées.

Notre démarche consiste à analyser les causes techniques et structurelles de ces biais, à évaluer leurs impacts sur les droits humains à travers des cas concrets, puis à examiner les réponses — réglementaires, industrielles et éthiques — qui ont été apportées à ce jour. Nous nous interrogeons enfin sur les conditions minimales qui rendraient l'usage de cette technologie éthiquement acceptable, ou sur la possibilité que ces conditions soient, dans certains contextes, tout simplement irréalisables.

---

## Problématique

La reconnaissance faciale est-elle éthiquement acceptable lorsqu'elle produit des résultats systématiquement discriminatoires selon la race et le genre ? Qui est responsable de ces biais — les concepteurs, les entreprises qui commercialisent ces outils, ou les États qui les déploient — et quels mécanismes de responsabilisation et de transparence permettraient de remédier à une discrimination algorithmique institutionnalisée ?

---

## Concepts clés

**Reconnaissance faciale.** La reconnaissance faciale est une technologie qui combine la biométrie, l'intelligence artificielle, la cartographie tridimensionnelle et l'apprentissage automatique pour identifier ou vérifier une personne à partir de son visage. Il est important de distinguer deux usages : la vérification (comparer un visage à une seule photo pour confirmer une identité revendiquée) et l'identification (comparer un visage à une base de données entière pour trouver une correspondance). C'est ce second usage, utilisé par les forces de l'ordre, qui pose le plus de problèmes éthiques car il implique une recherche massive dans des bases de données souvent constituées sans consentement explicite. La reconnaissance faciale fonctionne en extrayant les caractéristiques géométriques d'un visage — distance entre les yeux, forme du nez, contour de la mâchoire — puis en les convertissant en un vecteur numérique appelé « empreinte faciale », qui est ensuite comparé aux empreintes stockées dans une base de données. Sa définition, telle que proposée par l'Observatoire international de la reconnaissance faciale (OBVIA), insiste sur la dimension systémique de cette technologie, qui ne se réduit pas à un simple logiciel mais implique une infrastructure complète de collecte, de stockage et de traitement de données biométriques (OBVIA, 2021). Le Commissariat à la protection de la vie privée du Canada (2021) ajoute que cette technologie soulève des enjeux fondamentaux de consentement, de proportionnalité et de nécessité dans une société démocratique.

**Biais algorithmique.** Le biais algorithmique désigne une erreur systématique d'un algorithme qui produit des résultats inéquitables selon des caractéristiques démographiques telles que la race, le genre ou l'âge. Dans le contexte de la reconnaissance faciale, ce biais se manifeste par des écarts de précision significatifs entre les groupes démographiques. L'étude fondatrice Gender Shades de Buolamwini et Gebru (2018) a ainsi révélé que les systèmes de classification de genre les plus utilisés atteignaient un taux d'erreur de 34,7 % pour les femmes à peau foncée, contre 0,8 % pour les hommes à peau claire. Ces écarts ne résultent pas d'un défaut technique isolé mais d'un problème structurel : les données d'entraînement utilisées pour développer ces systèmes surreprésentent massivement les hommes aux teintes de peau claires — le jeu de données Labeled Faces in the Wild, l'un des plus utilisés, était composé à 77,5 % d'hommes et à 83,5 % de personnes à peau claire (Buolamwini et Gebru, 2018). Ce déséquilibre statistique conduit les algorithmes à être performants pour la population majoritaire dans les données d'entraînement, mais nettement moins pour les groupes sous-représentés. Comme le soulignent Pastaltzidis et al. (2024), ce biais n'est pas accidentel mais découle de choix de conception et de collecte de données qui reflètent des inégalités sociales préexistantes.

**Intersectionnalité.** L'intersectionnalité est un concept issu des études sur les discriminations, formalisé par la juriste Kimberlé Crenshaw, qui désigne la superposition de plusieurs axes d'identité — par exemple la race et le genre — qui amplifie les discriminations subies par les personnes se situant à l'intersection de ces catégories. Dans le cadre de la reconnaissance faciale, l'approche intersectionnelle adoptée par Buolamwini et Gebru (2018) a permis de révéler que les erreurs de classification n'étaient pas simplement plus fréquentes pour les femmes ou pour les personnes noires considérées séparément, mais qu'elles atteignaient leur niveau maximal pour les femmes noires, combinant ainsi les désavantages liés au genre et à la race. Cette approche est essentielle pour comprendre pourquoi les biais algorithmiques ne peuvent être analysés selon un seul axe d'identité, et pourquoi les solutions proposées doivent tenir compte de la complexité des identités sociales. Le concept d'intersectionnalité appliqué aux technologies de reconnaissance faciale montre que les préjudices ne sont pas distribués de manière uniforme : ils frappent plus durement celles et ceux qui cumulent plusieurs facteurs de marginalisation.

**Transparence algorithmique.** La transparence algorithmique renvoie à l'obligation de rendre intelligibles les processus et les décisions des systèmes automatisés, afin de permettre leur vérification, leur contestation et leur correction. Dans le domaine de la reconnaissance faciale, cette transparence est particulièrement difficile à atteindre en raison de la nature « boîte noire » de nombreux algorithmes d'apprentissage profond, dont le fonctionnement interne échappe même à leurs concepteurs. Wang et al. (2024) soulignent que la transparence constitue une condition préalable à toute réglementation efficace, car sans elle, il est impossible de démontrer qu'un système est équitable ou de contester ses décisions discriminatoires. Au Canada, la Loi 25 sur la protection des renseignements personnels dans le secteur privé impose déjà des obligations de transparence en matière de prise de décision automatisée, notamment le droit de savoir qu'une décision a été prise par un système automatisé et le droit de demander une révision humaine. Cependant, son application concrète à la reconnaissance faciale reste limitée, et la loi ne s'applique pas de manière uniforme aux forces de l'ordre (Loi 25, 2022). L'enjeu de la transparence rejoint directement celui de la responsabilité : sans capacité de comprendre et de vérifier le fonctionnement d'un algorithme, il est impossible de tenir quiconque responsable de ses erreurs.

---

## Méthodologie

Notre approche est analytique et empirique, structurée en deux temps complémentaires. Dans un premier temps, nous examinons les causes techniques des biais en nous appuyant sur les données empiriques du NIST (Grother et al., 2019), qui a testé environ 200 algorithmes de reconnaissance faciale et constitue la référence la plus complète en la matière, et sur l'étude Gender Shades (Buolamwini et Gebru, 2018), qui reste l'étude fondatrice du domaine. Nous analysons ensuite des cas concrets d'impacts réels — les arrestations injustifiées de Robert Williams (Détroit, 2020) et de Michael Oliver (Michigan, 2023) — documentés par l'ACLU et le Innocence Project, afin d'illustrer comment la discrimination algorithmique se traduit en préjudices concrets pour des personnes racisées. Une attention particulière est portée à la distinction entre les causes techniques des biais (données d'entraînement déséquilibrées, architecture des modèles) et les causes structurelles (inégalités sociales reproduites par la technologie).

Dans un second temps, nous évaluons les réponses éthiques et réglementaires existantes : la Déclaration de Montréal pour une IA responsable (2017), l'AI Act européen (2024), la Loi 25 québécoise (2022), le RGPD (Article 22) et les limites de ces cadres. Nous examinons également les réactions de l'industrie — les suspensions de vente aux forces de l'ordre annoncées par IBM, Microsoft et Amazon en 2020 — et leur insuffisance face à l'ampleur du problème. Le concept de blanchiment éthique (ethics washing), défini dans le cours, est mobilisé pour analyser le décalage entre les discours des entreprises et leurs pratiques réelles. Nous formulons enfin des recommandations sur les conditions minimales qui rendraient l'usage de cette technologie éthiquement acceptable, en nous appuyant sur les principes de responsabilité algorithmique et de transparence.

---

## Analyse

### Les mécanismes techniques à l'origine des biais

La reconnaissance faciale repose sur un processus en plusieurs étapes : acquisition de l'image, détection du visage, extraction des caractéristiques faciales (landmarks) et comparaison avec une base de données de référence. Chacune de ces étapes peut introduire des biais. Les biais algorithmiques s'insinuent principalement au niveau de l'entraînement du modèle d'apprentissage automatique. Lorsque les jeux de données utilisés pour entraîner un algorithme sont composés majoritairement de visages d'hommes blancs, le modèle apprend à reconnaître avec une grande précision ces visages, mais éprouve des difficultés avec ceux qui s'éloignent de cette norme statistique. Ce phénomène est aggravé par le fait que les algorithmes de deep learning sont conçus pour maximiser la précision globale, ce qui les conduit naturellement à optimiser leurs performances pour la majorité statistique au détriment des minorités.

Grother, Ngan et Hanaoka (2019), dans le cadre du Face Recognition Vendor Test (FRVT) du National Institute of Standards and Technology, ont testé environ 200 algorithmes commerciaux de reconnaissance faciale provenant de dizaines de fournisseurs à travers le monde. Leurs résultats sont sans équivoque : pour la majorité des algorithmes testés, les taux de faux positifs étaient significativement plus élevés pour les personnes noires que pour les personnes blanches, et plus élevés pour les femmes que pour les hommes. Dans le cas extrême de certains algorithmes, les taux de faux positifs pour les femmes noires étaient jusqu'à 100 fois supérieurs à ceux des hommes blancs. Ces écarts varient considérablement selon les algorithmes et les fournisseurs, ce qui démontre que le problème n'est pas inhérent à la technologie elle-même mais bien aux choix de conception et de données effectués par les développeurs. Le tableau suivant résume les principaux écarts observés par le NIST :

| Groupe démographique | Taux de faux positifs (médiane) | Écart par rapport au groupe de référence |
|---|---|---|
| Hommes blancs | 0,1 % | Référence |
| Femmes blanches | 0,3 % | 3x |
| Hommes noirs | 0,8 % | 8x |
| Femmes noires | 1,5 % | 15x |
| Femmes noires (pire algorithme testé) | Jusqu'à 10 % | 100x |

Ces résultats confirment que le problème ne réside pas dans un algorithme défectueux pris isolément mais dans un processus d'entraînement et de conception structurellement biaisé. Comme le soulignent Pastaltzidis et al. (2024) dans leur revue systématique des biais raciaux dans la reconnaissance faciale, les causes sont multiples : composition déséquilibrée des données d'entraînement, absence de diversité dans les équipes de conception, et manque de protocoles standardisés pour tester l'équité des systèmes avant leur déploiement.

### L'étude Gender Shades : une démonstration empirique fondatrice

L'étude Gender Shades, publiée en 2018 par Joy Buolamwini et Timnit Gebru au sein de la conférence FAT* (Fairness, Accountability, and Transparency), constitue le jalon empirique le plus influent dans la démonstration des biais de la reconnaissance faciale. Les deux chercheuses ont évalué trois systèmes commerciaux de classification de genre — ceux de Microsoft, IBM et Face++ — en utilisant un jeu de données appelé Pilot Parliaments Benchmark, composé de photos de parlementaires de plusieurs pays africains et européens, conçu spécifiquement pour assurer une représentation équilibrée selon la race et le genre. Chaque photo a été étiquetée manuellement selon le genre (homme, femme) et la pigmentation de la peau (plus claire, plus foncée), permettant ainsi une analyse intersectionnelle fine.

Les résultats furent alarmants et sans équivoque :

| Système | Hommes peau claire | Femmes peau claire | Hommes peau foncée | Femmes peau foncée |
|---|---|---|---|---|
| Microsoft | 0,0 % | 1,2 % | 0,3 % | 20,8 % |
| IBM | 0,3 % | 7,1 % | 0,7 % | 34,7 % |
| Face++ | 0,0 % | 1,0 % | 0,7 % | 34,5 % |

Comme le montre ce tableau, le système d'IBM présentait un taux d'erreur de 34,7 % pour les femmes à peau foncée, contre seulement 0,3 % pour les hommes à peau claire. Microsoft atteignait 20,8 % d'erreur pour les femmes à peau foncée, tandis que Face++ affichait 34,5 % pour cette même catégorie. L'originalité fondamentale de l'étude résidait dans son approche intersectionnelle : en croisant race et genre, les chercheuses ont montré que les erreurs n'étaient pas simplement réparties entre hommes et femmes, ou entre peaux claires et foncées, mais qu'elles se concentraient de façon disproportionnée sur les femmes noires, révélant ainsi une discrimination à l'intersection de deux axes d'identité (Buolamwini et Gebru, 2018). Cette étude a eu un impact considérable : elle a forcé IBM et Microsoft à améliorer leurs algorithmes (les versions ultérieures ont réduit mais n'ont pas éliminé les écarts), a conduit à la création d'un nouveau jeu de données plus équilibré, et a lancé un débat public mondial sur les biais de l'IA.

### Les cas Robert Williams et Michael Oliver : quand les biais deviennent des arrestations

Les conséquences des biais algorithmiques ne se limitent pas à des statistiques abstraites. Elles se traduisent en préjudices concrets et graves pour les personnes qui en sont victimes. Le cas de Robert Williams, survenu en janvier 2020 dans la ville de Détroit, est le premier cas public d'arrestation injustifiée directement liée à une erreur de reconnaissance faciale aux États-Unis. M. Williams, un homme noir de 42 ans, père de famille et technicien chez une compagnie aérienne, fut arrêté devant chez lui en présence de ses deux filles, âgées de 5 et 7 ans, par une douzaine de policiers armés. Le système de reconnaissance faciale utilisé par le département de police de Détroit avait confondu son visage avec celui d'un suspect de vol de montres de luxe, en se basant sur une image de surveillance de très mauvaise qualité. M. Williams fut détenu pendant 30 heures dans un commissariat, menotté, interrogé sans la présence d'un avocat, avant que les enquêteurs ne reconnaissent finalement l'erreur (ACLU, 2021).

En 2023, Michael Oliver, un homme noir de 35 ans, vécut une expérience similaire à Détroit. Arrêté à tort pour une agression qu'il n'avait pas commise, il fut détenu pendant plusieurs jours avant que la technologie de reconnaissance faciale ne soit reconnue comme défaillante. Sanford (2024), du Innocence Project, souligne que ces erreurs ne sont pas des accidents isolés mais la conséquence directe de systèmes dont la fiabilité varie considérablement selon la couleur de peau des personnes identifiées. L'organisation Innocence Project, traditionnellement focalisée sur les erreurs judiciaires liées aux témoignages oculaires et aux analyses ADN, a récemment élargi son champ d'action pour inclure les erreurs causées par l'intelligence artificielle, considérant qu'il s'agit d'une nouvelle source d'erreurs judiciaires systémiques. Ces deux cas illustrent ce que les chercheurs appellent les faux positifs : des erreurs d'identification qui, dans un contexte policier, se traduisent par des privations de liberté arbitraires, des atteintes à la dignité et une perte de confiance dans les institutions, et qui affectent de manière disproportionnée les personnes racisées.

### La réponse de l'industrie : suspension, mais pas renoncement

Face à la publication de l'étude Gender Shades, aux révélations du NIST et à la pression croissante de l'opinion publique et des mouvements sociaux (notamment dans le sillage du mouvement Black Lives Matter en 2020), plusieurs géants de la technologie ont annoncé des mesures concernant la vente de leurs outils de reconnaissance faciale aux forces de l'ordre. En juin 2020, IBM annonçait son retrait total du marché de la reconnaissance faciale, une décision saluée par les militants mais qui doit être nuancée : IBM était déjà un acteur moins important sur ce marché que ses concurrents. Le même mois, Amazon imposait un moratoire d'un an sur la vente de son service Rekognition aux forces de l'ordre, moratoire renouvelé par la suite sans être rendu permanent. Microsoft annonçait des mesures similaires.

Cependant, il est essentiel de mesurer la portée réelle de ces annonces. D'une part, elles ne concernent que la vente aux forces de l'ordre, laissant intact l'usage civil de ces technologies par les entreprises, les aéroports, les institutions financières et les gouvernements. D'autre part, les moratoires ont été assortis de conditions vagues et réversibles, et rien n'indique que les algorithmes aient été substantiellement améliorés entre-temps en ce qui concerne les biais raciaux et de genre. Comme le souligne la Nordic Journal of Human Rights (2023), ces décisions relèvent davantage de la gestion des risque de réputation que d'un véritable renoncement à un marché lucratif. L'industrie continue de développer et de commercialiser des systèmes de reconnaissance faciale pour des marchés toujours plus nombreux — contrôle d'accès physique, vérification d'identité bancaire, publicité ciblée, analyse des émotions en magasin — sans que les biais raciaux et de genre documentés par des études indépendantes aient été corrigés de manière satisfaisante.

### Blanchiment éthique et décalage entre discours et pratiques

Le concept de blanchiment éthique (ethics washing), défini dans le cadre du cours INM6000, est particulièrement pertinent pour analyser les réponses de l'industrie de la reconnaissance faciale. Le blanchiment éthique désigne l'instrumentalisation de l'éthique par une communication trompeuse, créant l'impression qu'une intelligence artificielle est éthique alors qu'aucune théorie, argument ou application éthique substantielle n'est en place et qu'aucun éthicien n'est impliqué. Ce concept s'inscrit dans la continuité de phénomènes bien connus comme l'écoblanchiment (greenwashing) en matière environnementale et le privacy washing en matière de protection des données.

Dans le secteur de la reconnaissance faciale, le blanchiment éthique se manifeste de plusieurs façons : des entreprises publient des principes éthiques ambitieux sans mettre en place les mécanismes de vérification correspondants ; elles financent des recherches sur l'équité algorithmique tout en continuant à commercialiser des systèmes dont les biais sont documentés ; elles créent des comités d'éthique internes sans pouvoir décisionnel réel. Comme le souligne la Déclaration de Montréal pour une IA responsable (2017), les principes éthiques ne valent que par leur mise en œuvre concrète. L'absence de mécanismes de contrôle indépendants et de sanctions en cas de non-respect des engagements permet à l'industrie de bénéficier de la légitimité conférée par le discours éthique sans en supporter les contraintes réelles.

### Les réglementations existantes : un cadre insuffisant

Plusieurs cadres réglementaires tentent d'encadrer l'usage de la reconnaissance faciale, mais leur portée reste limitée et leur application concrète est inégale. Le tableau ci-dessous résume les principales initiatives et leurs limites respectives :

| Cadre réglementaire | Portée | Obligations clés | Limites identifiées |
|---|---|---|---|
| **AI Act européen (2024)** | Interdiction de la RF en temps réel dans les espaces publics (sauf exceptions) ; autres usages classés à haut risque | Transparence, évaluation d'impact, supervision humaine, traçabilité | Entrée en vigueur progressive jusqu'en 2027 ; exceptions floues pour les forces de l'ordre |
| **Loi 25 québécoise (2022)** | Protection des renseignements personnels dans le secteur privé | Notification des décisions automatisées, droit à la révision humaine | Ne vise pas spécifiquement la RF ; ne s'applique pas aux forces de l'ordre |
| **RGPD — Article 22** | Droit de ne pas être soumis à une décision 100 % automatisée | Droit de recours, obligation d'intervention humaine | S'applique aux données personnelles, interprétation variable selon les États membres |
| **Déclaration de Montréal (2017)** | Principes volontaires pour le développement d'une IA responsable | Équité, bien-être, autonomie, prudence, responsabilité | Aucune force juridique contraignante ; adhésion volontaire |
| **Projets de loi américains** | Initiatives au niveau des États (ex : moratoires à San Francisco, Boston, Portland) | Interdiction pour les agences municipales | Absence de cadre fédéral uniforme ; patchwork législatif |

L'AI Act européen constitue le cadre le plus avancé à ce jour : il classe la reconnaissance faciale en temps réel dans les systèmes d'IA interdits, sauf dans des cas exceptionnels strictement encadrés de recherche de victimes ou de prévention de menaces terroristes imminentes. Pour les autres usages de la reconnaissance faciale, il impose des obligations de transparence, d'évaluation d'impact sur les droits fondamentaux et de supervision humaine. Au Canada, la Loi 25 impose des obligations de notification lorsque des décisions sont prises exclusivement par traitement automatisé, mais son champ d'application est limité au secteur privé. La Déclaration de Montréal formule dix principes — dont l'équité, la transparence et la responsabilité — mais il s'agit d'un engagement volontaire, sans force juridique contraignante. Ces cadres, bien que nécessaires, peinent à suivre le rythme du déploiement technologique et présentent des lacunes importantes en matière d'application concrète.

### La question de la responsabilité : entre concepteurs, déployeurs et régulateurs

La question de la responsabilité des biais algorithmiques est au cœur du débat éthique. Qui doit être tenu responsable des erreurs de reconnaissance faciale — les concepteurs de l'algorithme, les entreprises qui le commercialisent, ou les organisations (souvent des services de police) qui l'utilisent ? Le Cambridge Handbook of Facial Recognition in the Modern State (2024) propose une analyse en trois niveaux de la responsabilité algorithmique : la responsabilité technique (liée à la conception du modèle et au choix des données d'entraînement), la responsabilité organisationnelle (liée aux politiques de déploiement et à la formation des utilisateurs) et la responsabilité sociétale (liée aux impacts sur les droits humains et à la participation citoyenne).

Dans les cas de Robert Williams et Michael Oliver, la responsabilité fut diluée entre plusieurs acteurs : la police de Détroit invoqua la technologie comme un « outil d'investigation parmi d'autres », en rejetant la faute sur le fournisseur du logiciel ; les fournisseurs se réfugièrent derrière leurs conditions d'utilisation, qui précisent que leurs systèmes sont des « aides à la décision » et non des décideurs autonomes. Aucune sanction n'a été imposée à l'un ou l'autre des acteurs, et les victimes n'ont obtenu que des réparations partielles après des batailles juridiques prolongées. Cette dilution de la responsabilité constitue un obstacle majeur à la mise en œuvre de mécanismes de réparation efficaces et à l'établissement d'un véritable principe de responsabilité pour les dommages causés par les systèmes algorithmiques.

### Les limites de la correction technique

Une partie de l'industrie et de la recherche soutient que les biais algorithmiques peuvent être résolus par des améliorations techniques : en diversifiant les données d'entraînement, en développant des algorithmes plus robustes, en utilisant des techniques d'apprentissage automatique soucieuses de l'équité (fairness-aware machine learning), ou en appliquant des méthodes de prétraitement des données. Cependant, cette approche se heurte à des limites fondamentales qui remettent en question sa capacité à résoudre le problème à elle seule.

D'une part, l'équité algorithmique elle-même fait l'objet de désaccords profonds dans la communauté de recherche. Il n'existe pas de définition universellement acceptée de ce que signifie traiter « équitablement » différentes catégories de population. Comme le souligne le cours INM6000, on distingue au moins deux grandes familles de définitions : l'équité individuelle (un même résultat pour des profils similaires, indépendamment de l'attribut sensible) et l'équité de groupe (des statistiques agrégées comparables entre groupes). Or ces définitions sont mathématiquement incompatibles dans le cas général : un modèle parfaitement équitable au niveau individuel peut produire des résultats globalement déséquilibrés entre groupes si les groupes ont des profils de départ différents, et vice versa (Wang et al., 2024). Ce constat explique pourquoi il n'existe pas de consensus sur la notion d'équité algorithmique, ce qui permet à certaines entreprises de choisir arbitrairement une définition qui favorise leurs intérêts commerciaux sans justifier leur choix sur le plan éthique.

D'autre part, même un algorithme parfaitement équitable du point de vue statistique reste un système de surveillance de masse dont les implications pour la vie privée, la liberté d'expression et les droits fondamentaux sont considérables. Comme le souligne le Commissariat à la protection de la vie privée du Canada (2021), la reconnaissance faciale pose un défi structurel qui ne peut être réduit à un problème technique : il s'agit fondamentalement d'un enjeu de gouvernance démocratique et de droits humains. Le débat éthique ne porte donc pas seulement sur la précision des algorithmes, mais aussi sur la légitimité même de déployer à grande échelle une technologie qui transforme l'espace public en espace de surveillance.

---

## Conclusion

Ce projet a permis de démontrer que les biais algorithmiques dans la reconnaissance faciale ne constituent pas un simple défaut technique susceptible d'être corrigé par de meilleurs algorithmes, mais reflètent des inégalités structurelles que la technologie amplifie et institutionnalise. Les études de Buolamwini et Gebru (2018) et du NIST (Grother et al., 2019) ont établi empiriquement et de manière irréfutable l'existence de disparités significatives dans les performances des systèmes selon la race et le genre, tandis que les cas de Robert Williams (2020) et Michael Oliver (2023) ont montré les conséquences concrètes et graves de ces biais sur les droits fondamentaux des personnes racisées. Les réponses de l'industrie — moratoires partiels, suspensions conditionnelles, comités d'éthique sans pouvoir — relèvent en partie du blanchiment éthique, et les cadres réglementaires existants — AI Act européen, Loi 25 québécoise, Déclaration de Montréal — souffrent de lacunes importantes en matière d'application concrète et de sanction. La question de la responsabilité reste irrésolue, chaque acteur renvoyant la faute à un autre, au détriment des victimes qui peinent à obtenir réparation.

Plusieurs avenues de recherche future mériteraient d'être explorées. L'étude des mécanismes de régulation alternatifs, notamment les approches fondées sur les droits humains plutôt que sur la seule réglementation technique des algorithmes, pourrait offrir des pistes de solution plus robustes. L'évaluation longitudinale de l'impact réel des moratoires et des engagements volontaires de l'industrie sur l'équité des algorithmes permettrait de distinguer les mesures authentiques des opérations de blanchiment éthique. Enfin, la comparaison internationale des cadres réglementaires émergents (Europe, Canada, États-Unis) pourrait éclairer les pratiques les plus efficaces pour concilier innovation technologique et protection des droits fondamentaux. L'équipe considère que l'usage de la reconnaissance faciale en contexte policier, dans ses conditions actuelles de déploiement, pose un problème éthique fondamental qui ne peut être résolu par des ajustements techniques incrémentaux, mais nécessite une remise en question démocratique plus large de la place de cette technologie dans nos sociétés.

---

## Bibliographie

- Buolamwini, J. et Gebru, T. (2018). Gender Shades: Intersectional Accuracy Disparities in Commercial Gender Classification. *Proceedings of Machine Learning Research*, 81, 77–91. https://proceedings.mlr.press/v81/buolamwini18a.html

- Grother, P., Ngan, M. et Hanaoka, K. (2019). *Face Recognition Vendor Test (FRVT) Part 3: Demographic Effects*. NISTIR 8280. National Institute of Standards and Technology. https://nvlpubs.nist.gov/nistpubs/ir/2019/NIST.IR.8280.pdf

- Wang, X. et al. (2024). Beyond surveillance: privacy, ethics, and regulations in face recognition technology. *Frontiers in Big Data*, vol. 7. https://doi.org/10.3389/fdata.2024.1337465

- ACLU (2021). *Williams v. City of Detroit — Face Recognition False Arrest*. https://www.aclu.org/cases/williams-v-city-of-detroit-face-recognition-false-arrest

- Union européenne (2024). *Règlement sur l'intelligence artificielle (AI Act)*. Règlement UE 2024/1689. https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX:32024R1689

- OBVIA (2021). *Petit guide sur la reconnaissance faciale*. Observatoire international de la reconnaissance faciale. https://www.obvia.ca/petit-guide-sur-la-reconnaissance-faciale

- Commissariat à la protection de la vie privée du Canada (2021). *Fiches des enjeux — reconnaissance faciale*. https://www.priv.gc.ca/fr/protection-de-la-vie-privee-et-transparence-au-commissariat/divulgation-proactive/cpvp-parl-bp/ethi_frt_20210510/fe_frt_20210510/

- Sanford, A. (2024, 14 février). Artificial Intelligence Is Putting Innocent People at Risk of Being Incarcerated. *Innocence Project*. https://innocenceproject.org/news/artificial-intelligence-is-putting-innocent-people-at-risk-of-being-incarcerated/

- Cambridge University Press (2024). *The Cambridge Handbook of Facial Recognition in the Modern State*, Ch. 6. https://www.cambridge.org/core/books/cambridge-handbook-of-facial-recognition-in-the-modern-state/facial-recognition-technology-and-potential-for-bias-and-discrimination/B1C4A7F38AE00781EC8A559EFE48B3DF

- Pastaltzidis et al. (2024). Surveying Racial Bias in Facial Recognition. *Electronics*, 13(12). https://doi.org/10.3390/electronics13122317

- Auteur(s) (2023). Bias in Facial Recognition Technologies Used by Law Enforcement. *Nordic Journal of Human Rights*, vol. 42, no 2. https://doi.org/10.1080/18918131.2023.2277581

- Déclaration de Montréal pour une IA responsable (2017). Université de Montréal. https://declarationmontreal-iaresponsable.com
