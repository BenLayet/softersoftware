# Charte de contribution Softer Software

> **Version 0, brouillon.** Rédigée en français ; une version anglaise suivra une fois le texte stabilisé.
> Les passages marqués **À décider** ne sont pas encore tranchés. Les règles de rémunération attendent l'avis d'un juriste associatif.

## 1. Objet

Cette charte fixe la façon dont des logiciels sont demandés, financés, construits et validés, et dont l'argent reçu est reversé à celles et ceux qui les construisent.

Elle ne dépend d'aucune application. Card Games est le premier projet qui l'applique ; chaque application qui l'adopte y renvoie depuis son `CONTRIBUTING.md`.

## 2. Principes

1. **Utile.** On construit ce que des utilisateurs demandent, pour une raison qu'ils expriment.
2. **Juste prix.** Le prix d'une évolution correspond à l'effort de la construire, pas à ce que le marché peut supporter.
3. **Sans but lucratif.** Les sommes reçues servent à rémunérer les contributions et à couvrir les frais de fonctionnement, rien d'autre.
4. **Respect des personnes.** Pas de publicité, pas de revente de données, pas de mécanique d'achat incitative.
5. **Maintenable.** Une évolution ne doit pas rendre la suivante plus difficile ; une contribution qui dégrade la maintenabilité n'est pas acceptée.
6. **Transparent.** Demandes, estimations, validations et comptes sont publics.
7. **Libre de son outil.** On peut contribuer avec ou sans assistant de code.

## 3. Rôles

Une même personne peut tenir plusieurs rôles.

| Rôle | Fait | Décide |
| --- | --- | --- |
| Utilisateur | Utilise l'application | — |
| Demandeur | Décrit un besoin depuis l'application, signale un problème | La valeur de sa demande |
| Financeur | S'engage à payer pour une demande, ou donne librement | Quelles demandes il finance |
| Contributeur | Construit une story | L'effort annoncé de sa story |
| Validateur | Relit, accepte ou refuse, fusionne | L'acceptation et l'effort retenu |
| Association | Encaisse, tient et publie les comptes, verse les rémunérations | L'adoption et la modification de la charte |

Tant qu'il n'y a pas d'autre contributeur, Benjamin Layet est le seul validateur.

## 4. Cycle d'une demande

1. **Demande.** Le demandeur remplit le formulaire de l'application. La demande devient une issue du projet, gérée dans Clarée.
2. **Découpage.** La demande est découpée en stories : une personne, une intention, une raison. Chaque story est petite, testable et utile seule.
3. **Estimation.** Chaque story reçoit une valeur et un effort (section 5).
4. **Financement.** La demande est ouverte au financement. Elle n'est construite qu'une fois son seuil atteint (section 6).
5. **Construction.** Un contributeur prend une story, travaille sur une branche `stories/<numéro>-<titre>` et ouvre une pull request qui ferme la story.
6. **Validation.** Le validateur relit la pull request, fixe l'effort retenu, puis l'accepte ou la refuse.
7. **Publication.** Les stories acceptées sont publiées dans une version de l'application.
8. **Rémunération.** L'association verse aux contributeurs ce qui leur revient (section 7).
9. **Retour.** Les utilisateurs signalent ce qui manque ou ne va pas, ce qui crée de nouvelles demandes.

## 5. Valeur et effort

La valeur et l'effort se mesurent en **tailles**, sur l'échelle de Clarée :

| Taille | XXS | XS | S | M | L | XL |
| --- | --- | --- | --- | --- | --- | --- |
| Points | 1 | 2 | 3 | 5 | 8 | 13 |

- **Effort** : annoncé par le contributeur avant le travail, retenu par le validateur à l'acceptation. Il mesure la difficulté de la story, pas le temps passé ni l'outil utilisé.
- **Valeur** : ce que la story apporte aux utilisateurs. **À décider** : fixée par le demandeur, par les financeurs, ou par le validateur.
- Une story plus grande que XL est découpée.
- Valeur et effort sont portés par des labels `value:` et `effort:` sur l'issue.

## 6. Financement et seuil

- Le **coût** d'une demande est la somme des efforts de ses stories, multipliée par le prix d'un point d'effort. **À décider** : le prix d'un point.
- Les financeurs s'engagent sur un montant. La demande est construite quand la somme des engagements atteint son coût : c'est le **seuil**.
- Les dons libres, non liés à une demande, alimentent les frais de fonctionnement puis les demandes choisies par l'association.
- **À décider** : ce que deviennent les engagements d'une demande qui n'atteint jamais son seuil (annulation, report sur une autre demande, ou délai d'expiration).

## 7. Rémunération des contributions

- Seules les contributions **acceptées** sont rémunérées.
- Une contribution est rémunérée selon l'**effort retenu**, au prix du point d'effort fixé **avant** le début du travail.
- Les sommes reçues sont entièrement employées à rémunérer les contributions, après déduction des **frais de fonctionnement** (hébergement, frais de paiement, frais administratifs), publiés chaque année.
- **À décider, après avis juridique** :
  - le statut sous lequel un contributeur est payé (par exemple sur facture) ;
  - les règles applicables aux contributeurs qui sont aussi dirigeants de l'association ;
  - si le travail du validateur est rémunéré comme une contribution.

> Note : la doctrine fiscale française (BOI-IS-CHAMP-10-50-10-20) considère qu'une rémunération indexée sur le chiffre d'affaires est un indice de lucrativité, et limite la rémunération des dirigeants. C'est pourquoi la rémunération est fixée par l'effort et non par les recettes. Ce point doit être confirmé par un professionnel.

## 8. Validation

- Le validateur vérifie que la contribution fait ce que dit la story, qu'elle est testée, qu'elle respecte les règles du projet (son `README.md`, son `CLAUDE.md` le cas échéant) et qu'elle ne dégrade pas la maintenabilité.
- Un refus est motivé dans la pull request.
- Un désaccord sur l'effort retenu se règle dans la pull request ; **À décider** : l'instance d'appel quand il y aura plusieurs validateurs.
- La branche principale est protégée : seul un validateur peut fusionner.

## 9. Outils

- On peut contribuer avec ou sans assistant de code.
- Un contributeur qui utilise Claude Code sur le web le fait avec son propre abonnement. Ce coût reste à sa charge et n'entre pas dans l'effort.
- L'hébergement des applications est un détail d'implémentation, qui peut changer à tout moment.
- **À décider** : la licence du code des applications et les droits cédés par les contributeurs.

## 10. Transparence

- Les demandes, estimations et validations sont publiques dans les dépôts des projets.
- L'association publie au moins une fois par an ses recettes, ses frais de fonctionnement et les sommes versées à chaque contributeur. **À décider** : publication nominative ou par pseudonyme.

## 11. Modification de la charte

- La charte vit dans ce dépôt. Toute modification passe par une pull request.
- Tant que l'association n'existe pas, Benjamin Layet valide les modifications. Ensuite, la charte est adoptée et modifiée selon les statuts de l'association. **À décider** : l'adopter comme règlement intérieur.
- Une modification ne s'applique qu'aux demandes ouvertes après son adoption.
