# Gruppexamination-Airbean
## Decomposition

Vi började bryta ner alla huvudsidor i figma skissen sedan bröt vi ner dem bit för bit som vi kände var rimligt för att appen skulle fungera Vår tankeprocess var att få med alla huvud funktioner från  appstart till att den beställd en produkt.

Så om vi tar menyn sidan, som är väldigt viktig i denna appen, så var vi mer detaljerade en på en sida som ‘Om oss’. Vi la även till en sorterting / filtrerings och en sök funktion för det tycker vi låter rimligt.
Sedan kände vi att det fattades sidor som en kassa/checkout sida och även profil sida där man kan ändra saker och inte bara se sin orderhistorik.


## Pattern Recognition
Vi tänkte att dela in det i olika kategorier hjälpte oss att påbörja denna process.  

### Användare 
Det populära valen av en dryck ansåg vi borde hamna högre upp i listan beroende på vart efterfrågan ligger. Men är man inloggad borde förslagen vara det du normalt beställer sedan det mest populära.

### Funktioner
Vår tankeprocess var först att hitta funktionella patterns där hittade vi autentisiering som behövs under flera olika tillfällen exempelvis checkout, skapa konto, logga in osv.

### Layout
I layout hittade vi flera olika återkommande listor knappar iconer och formulär man skulle kunna återanvända exempelvis i kundvagnen har du en lista som är lik meny listan med andra storlekar. Iconer som meny icon och kundvagnsicon på flesta sidorna. och formulär för logga in och skapa konto.

## Algorithm design
I algoritm delen så tänkte vi att vi går igenom appen som en användare och lägger märke till vilka steg som behövs, var upprepade mönster hittas och vilka olika vägar vi har som leder till att en beställning har lagts.
“Lägga till mer?” loopen tänkte vi är till för att man ska kunna addera fler produkter innan man går vidare till kundvagnen vi tänkte ha välj produkter då kunde vi skippat loopen men vi valde att göra en loop för det känns mest rimligt. I kundvagnen la vi till en en loop så att man kan justera och ångra sig. När man bestämt sig har vi en validering som kollar om användaren är inloggad så att den slipper alla andra steg och tar sig direkt till vilken adress som kaffet ska fraktas till. Sen har vi 3 olika vägar gäst, skapa konto och logga in som tar dig till slutmålet via olika grenar.
