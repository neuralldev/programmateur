# programmateur
Script de génération des scénarii de Programmateur pour Jeedom

Creez un scénario par script portant le nom du fichier
Cochez la case <b>Active</b>, décochez <b>Visible</b>
Positionnez les script dans un groupe appelé <b>Chauffage</b>

Lancez le script <b>ChauffageEvalVariables</b> et cliquez sur <b>Voir Variables</b> pour vérifiez que les variables par défaut se sont bien créées dans la liste des variables globale de l'écran listant les scénarii. Si tout est correct vous devez avoir plusieurs variables avec le préfixe <b>Chaudière</b> disponibles : 

<table>
<th><td>Variable</td><td>Contenu</td><td>Commentaire</td></th>
<tr><td>ChaudiereThermostat</td><td>Nom complet d'objet Thermostat détecté par le script</td><td>Evalué automatiquement</td></tr>
<tr><td>ChaudiereDebutChauffe</td><td>Date de début de période de chauffe au format JJ/MM</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereFinChauffe</td><td>Date de fin de période de chauffe au format JJ/MM</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudierePeriodeChauffe</td><td>0 = pas en période de chauffe, 1 en période de chauffe</td><td>Evalué automatiquement</td></tr>
<tr><td>ChaudiereFerie</td><td>0 = normal, 1 jour férié</td><td>Evalué automatiquement</td></tr>
<tr><td>ChaudiereWeekEnd</td><td>0 = en semaine, 1 en eek-end</td><td>Evalué automatiquement</td></tr>
<tr><td>ChaudiereProgrammeStandard</td><td>Programme de la chaudiere pour les jours standards</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereProgrammeWeekEnd</td><td>Programme de la chaudiere pour les week-ends</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereProgrammeFeries</td><td>Programme de la chaudiere pour les jours fériés (hors week-ends)</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereDepartVacances</td><td>Mode à commuter en départ Vacances</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereRetourVacances</td><td>Mode à commuter en retour de Vacances</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereSortieNormale</td><td>Mode à commuter en sortie normale (mode absent)</td><td>peut être changé manuellement</td></tr>
<tr><td>ChaudiereRetourNormal</td><td>Mode à commuter en retour à l'état Présent (mode présent)</td><td>peut être changé manuellement</td></tr>

Une fois ce script enclenché, les autres sont à programmer selon les modes. Si l'objet Thermostat n'est pas détecté, les scripts ne peuvent pas fonctionner correctement. 

Cochez la case <b>Pas de log</b> une fois les vérification effectué pour limiter la verbosité et accélérer les traitements.

