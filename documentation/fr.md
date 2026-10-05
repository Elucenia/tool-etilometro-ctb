<!-- ELUCENIA technical documentation · etilometro-ctb · fr · no clinical/professional/rights approval -->

# Éthylomètre : valeur retenue (résolution brésilienne Contran 432)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/etilometro-ctb)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Mesure à l’éthylomètre (MR)

`mr`

mg/L d’air · intervalle: 0–5

## Édition de la méthode

CONTRAN 432/2013 annexe I : erreur 0,032/8%/30% ; troncature à 2 décimales ; application au Brésil

## Formule documentée

VC = MR − EM, à deux décimales, les autres étant supprimées (sans arrondi).

Erreur maximale admissible (EM) : MR inférieur à 0,40 mg/L = 0,032 mg/L ; MR de 0,40 à 2,00 mg/L = 8% de MR ; MR supérieur à 2,00 mg/L = 30% de MR.

Infraction (art. 165) : MR ≥ 0,05 mg/L (VC ≥ 0,01). Délit (art. 306) : MR ≥ 0,34 mg/L (VC ≥ 0,30 mg/L, équivalant à 6 dg/L dans le sang).

## Limites et population

La résolution 432/2013 distingue la mesure réalisée de la valeur retenue après déduction de l’erreur métrologique et exige un instrument approuvé et vérifié. La qualification admet aussi d’autres moyens, dont le sang et un ensemble de signes psychomoteurs. Un calcul d’éthylomètre seul ne constitue pas une évaluation clinique, une preuve d’aptitude à conduire ou une décision juridique ; l’applicabilité en vigueur du CTB et de la législation métrologique doit être vérifiée pour le cas.

## Références

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
