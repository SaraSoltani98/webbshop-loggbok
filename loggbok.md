# Individuell loggbok – Agil Webbshop

**Projekt:** Agil Webbshop  
**Period:** Vecka 39–44  
**Sprintar:** 1–6

---

## Sprint 1 – Vecka 39

### Vad jag arbetade med

Under den första sprinten började vi arbeta med vårt gemensamma projekt Agil Webbshop. Vi gick igenom projektets mål, planerade vilka funktioner som behövdes och delade upp arbetet mellan frontend och backend.

Jag började arbeta med frontend och bekantade mig med projektets struktur i React. Jag undersökte hur komponenter fungerar och hur vi skulle bygga upp webbshoppen.

Jag arbetade också med GitHub och lärde mig hur man använder branches, commits, push och pull för att samarbeta i samma projekt.

### Eventuella problem och hur jag löste dem

I början var det svårt att förstå hur frontend och backend skulle kommunicera med varandra.

Jag behövde också lära mig mer om projektstrukturen och hur vi skulle arbeta med GitHub utan att skapa konflikter i koden.

Jag försökte lösa problemen genom att läsa koden, testa olika saker och undersöka hur de olika delarna fungerade.

### Samarbete och agilt arbete

Under den första sprinten deltog jag i gruppens planering och fick bättre förståelse för det agila arbetssättet.

Vi använde en backlogg för att organisera våra uppgifter och planerade vad vi skulle fokusera på under sprinten.

Jag lärde mig att det är viktigt att dela upp stora uppgifter i mindre delar och kommunicera med gruppen.

---

## Sprint 2 – Vecka 40

### Vad jag arbetade med

Under den här sprinten arbetade jag med frontend och autentisering.

Jag arbetade med att koppla frontend till vår auth-service för att användare skulle kunna logga in i webbshoppen.

Jag arbetade också med att hantera roller för inloggade användare, till exempel ADMIN och USER.

Syftet var att systemet skulle kunna identifiera vem som var inloggad och vilken behörighet användaren hade.

Jag arbetade med att visa rätt information och funktioner beroende på användarens roll.

Jag arbetade även med olika delar av frontend för att förbättra hur webbshoppen fungerade.

### Eventuella problem och hur jag löste dem

En utmaning var att förstå hur autentisering fungerar mellan frontend och backend.

Jag behövde undersöka hur frontend kunde få information om den inloggade användaren och hur rollen skulle användas för att styra vilka funktioner som visades.

Jag testade inloggningen och undersökte hur API-anropen fungerade.

Genom detta fick jag bättre förståelse för hur autentisering och behörigheter fungerar i en webbapplikation.

### Samarbete och agilt arbete

Under sprinten fortsatte vi att arbeta med våra uppgifter i sprintbackloggen.

Jag lärde mig att frontend och backend måste samarbeta för att inloggningen och rollerna ska fungera korrekt.

Det var viktigt att kommunicera med gruppen om vilka API-anrop och vilken användarinformation frontend behövde.

---

## Sprint 3 – Vecka 41

### Vad jag arbetade med

Under den här sprinten arbetade jag med att förbättra användargränssnittet och produktfunktionerna i webbshoppen.

En av uppgifterna var att ta bort en extra utloggningsknapp eftersom vi hade två logout-knappar.

Jag tog bort den dubbla knappen så att användaren bara skulle se en tydlig utloggningsknapp.

Jag arbetade också med funktionen som gör att användaren kan klicka på en produkt och se mer information om den.

Syftet var att kunden skulle kunna öppna en produkt och se dess detaljer innan ett eventuellt köp.

Det här arbetet hjälpte mig att förstå mer om React-komponenter, produktdata och navigering mellan olika vyer.

### Eventuella problem och hur jag löste dem

Ett problem var att webbshoppen hade dubbla utloggningsknappar, vilket gjorde gränssnittet mindre tydligt.

Jag undersökte var knapparna visades och arbetade med att ta bort den onödiga knappen.

Jag behövde också förstå hur vi kunde visa information om en specifik produkt när användaren klickade på den.

Genom att undersöka komponenterna och hur produktinformationen hanterades kunde jag arbeta vidare med funktionen.

### Samarbete och agilt arbete

Under sprinten arbetade jag med konkreta uppgifter som förbättrade användarupplevelsen.

Jag lärde mig att även mindre förbättringar är viktiga för slutresultatet.

Genom att dela upp arbetet i mindre uppgifter kunde jag fokusera på en funktion i taget och kontrollera resultatet.

---

## Sprint 4 – Vecka 42

### Vad jag arbetade med

Under den här sprinten arbetade jag med en funktion för administratören och med en undersökning av betalningslösningar.

Jag arbetade med att göra det möjligt för admin att ladda upp bilder till produkter.

Syftet var att administratören skulle kunna lägga till produktbilder och göra produkterna tydligare för kunderna.

Jag fick arbeta med filuppladdning i frontend och förstå hur bildinformation ska skickas och hanteras.

Jag arbetade också med uppgiften **Undersök betalning för webbshoppen**.

Jag undersökte tre olika betalningslösningar:

- Stripe
- Klarna
- Swish

**Stripe:** Jag undersökte hur Stripe Checkout fungerar, hur backend kan skapa en Checkout Session och hur man kan testa betalningar med testkort utan riktiga pengar. Jag såg att Stripe har bra dokumentation och en färdig checkout-sida, men kräver API-nycklar och hantering av betalningsstatus.

**Klarna:** Jag undersökte hur Klarna kan användas för direktbetalning, betala senare och delbetalning. Jag läste om Klarnas testmiljö Playground och hur backend behöver kommunicera med Klarnas API.

**Swish:** Jag undersökte hur en betalning kan startas från webbshoppen och godkännas i Swish-appen. Jag såg att Swish är ett vanligt betalningsalternativ i Sverige, men att integrationen kräver mer teknisk konfiguration.

Jag dokumenterade fördelar, nackdelar, testmiljöer och vad som skulle behövas i frontend och backend.

### Eventuella problem och hur jag löste dem

En utmaning med bilduppladdningen var att förstå hur frontend ska hantera en bildfil och skicka den vidare till backend.

När jag undersökte betalningslösningarna upptäckte jag att de fungerar på olika sätt och har olika krav.

Det var särskilt viktigt att förstå skillnaden mellan vad frontend ska göra och vad backend ansvarar för.

Jag använde dokumentationen från Stripe, Klarna och Swish för att undersöka alternativen och jämföra deras fördelar och nackdelar.

Betalningsuppgiften var en undersökning och ingen färdig integration.

### Samarbete och agilt arbete

Under den här sprinten fick jag bättre förståelse för varför undersökning och planering är viktiga delar av agil utveckling.

Innan man börjar utveckla en större funktion behöver man förstå vilka alternativ som finns och vilka tekniska krav som gäller.

Min betalningsundersökning kunde användas som underlag när gruppen skulle diskutera en framtida betalningslösning.

Jag lärde mig också att vissa uppgifter kräver samarbete mellan frontend och backend.

---

## Sprint 5 – Vecka 43

### Vad jag arbetade med

Under den här sprinten arbetade jag med tester i frontend.

Jag använde **Vitest och MSW (Mock Service Worker)** för att testa webbshoppens funktioner.

Vitest användes för att köra automatiserade tester och kontrollera att funktioner och komponenter fungerade som förväntat.

Jag arbetade även med MSW för att simulera API-anrop och skapa testsvar.

Med MSW kunde jag testa frontend utan att alltid behöva vara beroende av att backend var igång.

Jag fortsatte också att arbeta med olika delar av frontend och undersöka hur funktionerna samverkade.

### Eventuella problem och hur jag löste dem

I början var det svårt att förstå hur testerna skulle skrivas och hur MSW skulle användas.

Jag behövde lära mig hur man simulerar API-svar och hur tester kan kontrollera att frontend visar rätt information.

Jag undersökte testkoden och testade olika lösningar för att förstå hur verktygen fungerade.

Genom arbetet fick jag bättre kunskaper om automatiserade tester och varför de är viktiga för kodens kvalitet.

### Samarbete och agilt arbete

Under sprinten förstod jag bättre hur tester kan hjälpa hela teamet.

Om vi testar funktionerna regelbundet kan vi upptäcka problem tidigare och minska risken för att nya ändringar förstör befintliga funktioner.

Jag lärde mig att testning är en viktig del av utvecklingsarbetet och att det inte räcker att bara skriva kod.

Jag fick också bättre förståelse för hur man kan arbeta stegvis och kontrollera resultatet under en sprint.

---

## Sprint 6 – Vecka 44

### Vad jag arbetade med

Under den här sprinten arbetade jag med att testa och felsöka vår webbshop efter att den hade publicerats på Render.

Jag kontrollerade olika funktioner i frontend, bland annat inloggningen och produktvisningen.

När jag loggade in som administratör fungerade inloggningen, men produkterna visades inte.

Jag fick felmeddelandet:

**429 Too Many Requests**

Jag började undersöka problemet med hjälp av Chrome DevTools.

Jag öppnade fliken Network och kontrollerade vilka API-anrop som skickades från frontend.

Jag såg att anropet till `/me` gav status 200, medan anropet till `/products` gav status 429.

Jag undersökte även Headers och Response för att se vilken server som svarade och vilken endpoint som orsakade felet.

### Eventuella problem och hur jag löste dem

Det största problemet var att webbshoppen inte kunde hämta produkterna.

Jag upptäckte att anropet till vår API Gateway:

`https://gateway-agil.onrender.com/products`

gav status 429.

Det betyder att servern avvisade förfrågan på grund av en begränsning av antalet anrop.

Jag undersökte om felet kunde bero på frontend, backend eller API Gateway.

Genom felsökningen kunde jag identifiera var felet visade sig, men jag hade ännu inte fastställt den exakta orsaken.

Nästa steg var att kontrollera Gateway-konfigurationen och loggarna i Render.

### Samarbete och agilt arbete

Under sprinten lärde jag mig att det är viktigt att testa webbshoppen som en helhet.

Även om en funktion fungerar lokalt kan det uppstå problem när frontend och backend körs på olika tjänster.

Jag arbetade steg för steg för att undersöka felet och få fram information som kunde hjälpa oss att lösa problemet.

Jag lärde mig också vikten av att dokumentera fel, prioritera viktiga problem och följa upp dem i kommande sprintar.

---

# Sammanfattning av mitt individuella arbete

Under projektet Agil Webbshop har jag arbetat med flera olika delar av frontend och fått bättre förståelse för hur en webbapplikation fungerar.

Mina viktigaste arbetsuppgifter har varit:

- Utveckling och förbättring av frontend i React.
- Arbete med autentisering och inloggning via auth-service.
- Hantering av användarroller som ADMIN och USER.
- Borttagning av en dubbel logout-knapp.
- Funktion för att visa produktdetaljer när användaren klickar på en produkt.
- Funktion för att admin ska kunna ladda upp produktbilder.
- Undersökning av betalningslösningarna Stripe, Klarna och Swish.
- Arbete med automatiserade tester med Vitest och MSW.
- Felsökning av API-anrop och HTTP-status 429.

Jag har utvecklat mina kunskaper inom React, autentisering, API-kommunikation, testning och felsökning.

Jag har också lärt mig mer om agilt arbete, planering och hur viktigt det är att samarbeta i ett projekt där frontend och backend är beroende av varandra.

# Vad jag har lärt mig och vill förbättra

Det viktigaste jag har lärt mig är att programmering inte bara handlar om att skriva kod utan också om att förstå problem, testa lösningar och förbättra funktioner.

Jag har blivit bättre på att undersöka hur olika delar av en webbapplikation fungerar tillsammans.

Jag har också förstått varför tester är viktiga och hur verktyg som Vitest och MSW kan hjälpa oss att upptäcka problem tidigare.

Genom betalningsundersökningen har jag fått förståelse för hur externa betaltjänster kan integreras i en webbshop.

Framöver vill jag bli ännu bättre på React, API-integrationer och automatiserade tester. Jag vill också utveckla min förmåga att självständigt felsöka problem och hitta lösningar.
