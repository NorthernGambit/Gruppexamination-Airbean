# Gruppexamination – Airbean

## Figma-Skiss
https://www.figma.com/board/wHeMgbHO5Lm0OWbzy4flUy/Airbean?node-id=55-616&t=vYPvqMoh6MfDimIx-1

## Decomposition

Vi började med att bryta ner alla huvudsidor i Figma-skissen. Sedan bröt vi ner dem bit för bit, vilket vi kände var rimligt för att appen skulle fungera. Vår tankeprocess var att få med alla huvudfunktioner, från app-start till att en produkt är beställd.

Om vi tar menysidan, som är väldigt viktig i denna app, så var vi mer detaljerade än på en sida som ”Om oss”. Vi la även till sortering/filtrering och en sökfunktion, för det tyckte vi lät rimligt.
Sedan kände vi att det fattades sidor, som en kassa/checkoutsida och även en profilsida där man kan ändra saker och inte bara se sin orderhistorik.

## Pattern Recognition
Vi tänkte att indelningen i olika kategorier hjälpte oss att påbörja denna process.

### Användare
De populära valen av dryck ansåg vi borde hamna högre upp i listan, beroende på var efterfrågan ligger. Men är man inloggad borde förslagen vara det du normalt beställer, följt av det mest populära.

### Funktioner
Vår tankeprocess var först att hitta funktionella patterns. Där hittade vi autentisering som behövs vid flera olika tillfällen, exempelvis i checkout, när man skapar konto, loggar in osv.

### Layout
I layouten hittade vi flera olika återkommande listor, knappar, ikoner och formulär man skulle kunna återanvända. Exempelvis har du i kundvagnen en lista som är lik menylistan men med andra storlekar. Det finns ikoner som menyikon och kundvagnsikon på de flesta sidorna, samt formulär för att logga in och skapa konto.

## Abstraction
Under abstraction så valde vi ut de väsentliga delarna av appen och bröt ner dem till minsta möjliga beståndsdelar. Vad behövs för att visa en produkt? Vad behöver sparas för att en användare ska ha ett konto? Med det tankesättet gick vi igenom alla punkter och kom fram till den lista vi har.

## Algorithm design
I algoritmdelen tänkte vi att vi går igenom appen som en användare och lägger märke till vilka steg som behövs, var upprepade mönster hittas och vilka olika vägar vi har som leder till att en beställning har lagts.

”Lägga till mer?”-loopen tänkte vi är till för att man ska kunna addera fler produkter innan man går vidare till kundvagnen. Vi tänkte att om vi haft ”välj produkter” så kunde vi skippat loopen, men vi valde att göra en loop för det kändes mest rimligt. I kundvagnen la vi till en loop så att man kan justera och ångra sig. När man bestämt sig har vi en validering som kollar om användaren är inloggad, så att denne slipper alla andra steg och tar sig direkt till valet av vilken adress kaffet ska fraktas till. Sen har vi tre olika vägar: gäst, skapa konto och logga in, som tar dig till slutmålet via olika grenar.
