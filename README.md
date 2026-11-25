# Mutual Connect TEST

Environnement de test de Mutual Connect. Rien de ce qui est fait ici ne touche la production.

- Adresse : https://glvq1.github.io/mutual-connect-test/
- Back-end : copie du projet Apps Script, avec ses propres classeurs (données fictives)
- Bandeau orange et icône « TEST » pour ne pas confondre avec l'appli de production
- Notifications push désactivées, pour ne jamais en envoyer aux appareils de production
- Stockage local et cache du service worker préfixés `mc_test_` / `mutual-test-shell-` (tous les sites glvq1.github.io partagent la même origine)

## Circuit d'un changement

1. Le changement est fait ici (ou sur une branche) et testé sur tablette.
2. Une fois validé, il est reporté dans `glvq1/mutual-connect` (production).

## Réglage

L'URL `/exec` de la copie Apps Script de test est dans `index.html` (attribut `data-src` de l'iframe).
