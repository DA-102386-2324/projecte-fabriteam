# Enunciat del Projecte 2324

## Descripció de l'Activitat:

Els participants en aquest projecte han de desenvolupar una aplicació Android (JAVA) basada en el joc "Lines & Dots". La implementació ha de seguir els principis de l'arquitectura MVVM, incorporar databindings per a la interfície d'usuari, integrar Firebase per a la persistència de dades, i incloure proves unitàries per garantir la robustesa del codi.

## Context

El joc "Lines & Dots" té les seves arrels en un joc tradicional que Édouard Lucas, un matemàtic francès, va descriure per primera vegada al segle XIX. Aquest joc clàssic de llapis i paper és simple i entretingut, dissenyat per a 2 o més jugadors.

Les regles bàsiques impliquen dibuixar línies entre punts adjacents per formar quadrats i guanyar punts. La graella pot ser de qualsevol mida i la victòria es determina pel jugador amb més quadrats tancats al final de la partida.

Es recomana veure aquest vídeo explicatiu de les regles i com es juga: [Dots and Boxes](https://www.youtube.com/watch?v=FKv5KBzFW_s).

### Regles Bàsiques del Joc

* Cada torn, un jugador ha de dibuixar una línia entre punts adjacents horitzontalment o verticalment.
* La línia dibuixada ha d'estar disponible i no haver estat dibuixada anteriorment.
* Cada jugador disposa d'un únic moviment per torn.
* El jugador que completa un quadrat guanya un punt i obté un moviment addicional en aquell torn.
* El joc continua fins que es tanquen tots els quadrats, i el jugador amb més quadrats tancats guanya.

## Requisits Funcionals

1. **Login i Registre d'Usuari:**
   - Implementar una pantalla d'inici de sessió i registre amb Firebase Authentication.
   - Validar i gestionar el registre d'usuaris.
   - Afegir una SplashScreen amb el logo del joc.

2. **Creació d'un Tema Propi:**
   - Proporcionar un tema personalitzat, incloent tipografia i paleta de colors.
   - Documentar el tema en format Markdown.

3. **Implementació del Joc:**
   - Desenvolupar la lògica del joc "Lines & Dots" amb la possibilitat de jugar contra un bot.
   - Permetre partides de n jugadors.
   - Permetre als jugadors triar el seu color en cada partida, assegurant que cada jugador tingui un color únic.
   - Permetre la selecció de la mida del taulell per a cada partida.
   - Implementar un mecanisme per determinar quin jugador comença (a través d'un dau, pedra-paper-tisora, etc.).
   - Habilitar la connexió a partides multijugador mitjançant Firebase Realtime Database per sincronitzar l'estat del joc entre dispositius.
   - Gestionar els torns dels jugadors i registrar els seus moviments.

4. **Ranking de Jugadors:**
   - Desenvolupar una funcionalitat de ranking que mostri els millors jugadors registrats.
   - Utilitzar Firebase per emmagatzemar les puntuacions dels jugadors.

5. **Perfil d'Usuari:**
   - Crear una pàgina de perfil d'usuari on els jugadors puguin consultar les seves estadístiques i historial de partides.
   - Utilitzar Firebase per emmagatzemar la informació del perfil.

A més a més, podeu afegir i complementar aquesta base amb les funcionalitats que desitjeu.

## Avaluació 

L'avaluació es basa en un 50% de criteris qualitatius i un 50% de criteris quantitatius. Els criteris qualitatius segueixen les pautes de la rúbrica següent:

### Rúbrica d'Avaluació

| **Mètrica**           | **Excel·lent (6p)**  | **Molt Bé (4p)**  | **Acceptable (2p)**  | **Insatisfactori (0p)**  |
|----------------------|----------------------|-------------------|----------------------|--------------------------|
| *Desenvolupament del Programa* | El programa compila sense errors lògics i supera les especificacions. | El programa compila sense errors lògics i compleix les especificacions. | El programa compila amb alguns errors mínims i compleix la majoria de les especificacions. | El producte produeix resultats incorrectes i/o no compila en absolut i no compleix la majoria de les especificacions. |
| *Modularitat* | El programa està descompost en unitats coherents i reutilitzables, i s'ha eliminat la repetició innecessària. | El programa està descompost en unitats coherents, tot i que pot contenir algunes repeticions innecessàries. | El programa està descompost en unitats de mida adequada, però manquen coherència o reutilització. El codi conté repeticions innecessàries. | El programa conté funcions massa grans o està descompost de manera que té poc sentit. |
| *Claredat* | El projecte conté documentació adequada per a totes les funcions principals, variables o algorismes no trivial. El codi es pot llegir amb facilitat. | El programa conté alguna documentació. Bona format i estil. Però la lectura no és fluïda. | El programa conté alguna documentació. No obstant això, l'estil i el format no són apropiats per a una bona lectura. | El programa no conté documentació o és impossible de llegir a causa de l'estil o el format. |
| *Patrons de Disseny* | El codi utilitza patrons de disseny i principis adequats. | El codi utilitza patrons i alguns bons principis de disseny. | El codi utilitza patrons, però no sempre de la manera adequada. | El codi no utilitza cap patró ni principis de disseny. |
| *Eficiència* | El codi és extremadament eficient sense sacrificar la llegibilitat i la comprensió. | El codi és bastant eficient sense sacrificar la llegibilitat i la comprensió. | El codi utilitza la força bruta, malgasta recursos i/o és innecessàriament llarg. | El codi és enorme i està unit sense tenir en compte l'eficiència en termes de recursos. |
| *Completitud* | El projecte mostra evidència d'una anàlisi excel·lent dels casos, i tots els casos possibles es gestionen adequadament. | Els programes mostren evidència d'una anàlisi de casos que és gairebé completa, però pot haver deixat passar casos menors o inusuals. | El programa mostra certa evidència d'anàlisi de casos, però potser es perden casos significatius o hi ha errors en el tractament d'alguns escenaris. | El programa rarament gestiona casos diferents o mostra errors en l'anàlisi de casos. |

Els criteris quantitatius es basen en els requisits funcionals:

1. Jugabilitat (Regles del joc i desenvolupament de la partida) (fins a 20 punts)
2. Funcionalitat de registre (fins a 10 punts)
3. Funcionalitat de login (fins a 10 punts)
4. Funcionalitat de perfil d'usuari (fins a 10 punts)
5. Partides contra bots (fins a 10 punts)
6. Partides multijugador (fins a 20 punts)
7. Rànquing de jugadors (fins a 10 punts)
8. Documentació (fins a 10 punts)