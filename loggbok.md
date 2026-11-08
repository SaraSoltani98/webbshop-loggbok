# Individuell loggbok – Webbshop

Vi har arbetat i enveckas-sprintar och följt ett agilt arbetssätt med sprintplanering, dagliga avstämningar, sprint review och retro. Vi har använt Trello för att hantera backloggen och GitHub med branches och pull requests för vårt kodarbete.

---

## Sprint 1 – vecka 39

### Vad jag arbetade med

Under den första sprinten arbetade jag med **FE-04 – Alla kan köra frontend lokalt**, som var en gemensam uppgift för hela gruppen.

Jag klonade frontendprojektet från GitHub, installerade de beroenden som behövdes och fick React-applikationen att fungera lokalt på min dator.

Jag klonade även projektets olika mikrotjänster för att börja förstå hur hela systemet var uppbyggt. Jag började sätta mig in i hur frontend, auth-service, product-service och order-service skulle kommunicera med varandra.

Under den här sprinten lärde jag mig också mer om Git, GitHub och hur vi skulle arbeta med branches i projektet.

### Utmaningar och lösningar

I början var en utmaning att förstå hur alla projekt skulle startas och vilka portar de olika tjänsterna använde.

Jag testade därför tjänsterna en i taget och kontrollerade att de kunde starta lokalt innan jag gick vidare. På så sätt fick jag bättre förståelse för projektstrukturen och vilka kommandon som behövdes för frontend och backend.

### Samarbete och agilt arbete

På måndagen hade vi sprintplanering där vi gick igenom backloggen och fördelade uppgifterna mellan oss.

Under veckan hade vi dagliga avstämningar där vi berättade vad vi arbetade med, vad vi skulle göra härnäst och om vi hade stött på några problem.

Vi använde Trello för att följa vilka uppgifter som var pågående och vilka som var färdiga. På fredagen hade vi sprint review där vi visade läraren vad vi hade gjort under veckan.

---

## Sprint 2 – vecka 40

### Vad jag arbetade med

Under den här sprinten började jag arbeta mer med **auth-service**, som blev mitt huvudsakliga ansvarsområde i projektet.

Jag arbetade med **FE-08 – Returnera inloggningsdata som DTO**. Vid inloggning behövde auth-service returnera mer information om användaren, bland annat token, användarnamn och roller.

Jag arbetade även med **FE-10 – Visa välkomstsida efter inloggning**. Jag kopplade informationen från auth-service till frontend så att det gick att visa vem som var inloggad och vilken roll användaren hade.

Jag arbetade också med rollerna `USER` och `ADMIN` och började få en bättre förståelse för JWT och autentisering.

### Utmaningar och lösningar

En utmaning var att förstå hur informationen som skickades från auth-service skulle användas i frontend.

Jag behövde förstå hur JWT-token, användarinformation och roller hängde ihop. Jag testade därför inloggningsflödet steg för steg och kontrollerade vad auth-service faktiskt returnerade.

När jag hade förstått hur svaret var uppbyggt kunde jag koppla rätt information till frontend.

### Samarbete och agilt arbete

Under sprintplaneringen gick vi igenom vilka delar som behövdes för att få inloggningsflödet att fungera.

På våra dagliga avstämningar diskuterade vi hur frontend och backend skulle kopplas ihop. Eftersom auth-service användes av flera delar i systemet behövde jag kommunicera med gruppmedlemmarna om hur inloggningssvaret fungerade.

På sprint review kunde vi visa hur autentisering och användarinformation fungerade.

---

## Sprint 3 – vecka 41

### Vad jag arbetade med

Jag fortsatte arbeta med auth-service och integrationen mellan frontend och backend.

Jag arbetade med att visa användarens roller och vem som var inloggad genom funktionaliteten i auth-service.

Jag arbetade också med **FE-25 – Frontend ska kunna visa imageUrl för produkter** och med produktvisningen i frontend.

Jag arbetade även med funktionen där användaren kan klicka på ett produktkort och komma till en detaljvy för den aktuella produkten.

Under sprinten deltog jag också i arbetet med att kontrollera att **email-service kunde köras lokalt**.

Jag fortsatte dessutom att köra de olika mikrotjänsterna lokalt för att få bättre förståelse för hur de kommunicerade med varandra.

### Utmaningar och lösningar

En utmaning var att de olika mikrotjänsterna använde olika portar och hade olika konfigurationer.

Jag behövde förstå vilken tjänst som skulle anropa vilken annan tjänst och på vilken port.

För att felsöka testade jag först tjänsterna separat och sedan tillsammans. Det gjorde det lättare att hitta var ett fel uppstod.

Under den här sprinten blev jag mer van vid att felsöka ett system som består av flera mikrotjänster.

### Samarbete och agilt arbete

Vi fortsatte använda Trello för att följa våra uppgifter.

Under våra dagliga avstämningar berättade vi vad vi arbetade med och om någon hade problem som blockerade arbetet.

Eftersom flera funktioner var beroende av varandra behövde vi hjälpa varandra med testning och integration mellan tjänsterna.

På sprint review gick vi igenom de funktioner som hade blivit färdiga.

---

## Sprint 4 – vecka 42

### Vad jag arbetade med

Under den här sprinten arbetade jag med **FE-14 – Undersök betalning för webbshoppen**.

Jag undersökte olika betalningslösningar och tittade bland annat på **Klarna och Swish** för att förstå hur de skulle kunna användas i vår webbshop.

Jag undersökte hur ett betalningsflöde skulle kunna fungera och vilka delar som skulle behöva hanteras i frontend och backend.

Jag skapade även ett dokument i frontendprojektet där jag dokumenterade det jag hade undersökt om betalningslösningarna, så att gruppen kunde ta del av informationen.

Syftet med uppgiften var framför allt att undersöka och förstå möjliga betalningslösningar, inte att implementera en färdig betalningsfunktion.

Jag fortsatte samtidigt att arbeta med auth-service och lokal testning av mikrotjänsterna.

Jag testade hur frontend, auth-service, product-service och order-service fungerade tillsammans och började få en bättre förståelse för hur autentisering behöver fungera när flera mikrotjänster är inblandade.

Under den här perioden började vi också diskutera behovet av en gemensam gateway.

### Utmaningar och lösningar

En utmaning med betalningsuppgiften var att förstå hur externa betalningslösningar som Klarna och Swish skulle kunna kopplas till vårt system.

Jag behövde undersöka vad som skulle ske i frontend och vad som skulle behöva hanteras i backend. Genom att läsa, testa och dokumentera alternativen fick jag en bättre förståelse för hur ett betalningsflöde kan byggas upp.

En annan utmaning var att det började bli många olika adresser och portar att hålla reda på när frontend kommunicerade med flera mikrotjänster.

Det gjorde felsökningen svårare eftersom ett fel kunde ligga i frontend, CORS-konfigurationen eller i någon av backend-tjänsterna.

Jag lärde mig därför att felsöka steg för steg genom att först kontrollera att varje tjänst fungerade separat och sedan testa kommunikationen mellan tjänsterna.

### Samarbete och agilt arbete

Under sprintplaneringen valde vi betalningslösningen som en undersökningsuppgift.

Jag dokumenterade det jag kom fram till så att resten av gruppen kunde ta del av resultatet.

Under våra avstämningar diskuterade vi hur en framtida betalningslösning skulle kunna passa in i systemet och hur vår arkitektur kunde förbättras.

Vi började också diskutera behovet av att samla kommunikationen mellan frontend och backend genom en gateway.

På sprint review kunde vi visa vad som hade undersökts även om någon färdig betalningsintegration inte implementerades.

---

## Sprint 5 – vecka 43

### Vad jag arbetade med

Under den här sprinten arbetade jag med **FE-32 – Gateway-applikation i backend**.

Alla i gruppen fick skapa en egen gateway för att lära oss hur en gateway och reverse proxy fungerar.

Jag skapade och testade min egen lösning för att förstå hur requests från frontend kunde skickas vidare till rätt mikrotjänst.

Efter att vi hade testat våra olika lösningar jämförde vi dem i gruppen och valde en gemensam gateway som skulle användas i projektet.

Jag klonade sedan den gemensamma `gateway-agil` och började köra den tillsammans med de andra mikrotjänsterna lokalt.

Jag körde auth-service, product-service, order-service, gateway och frontend tillsammans för att testa hur hela systemet fungerade.

Jag arbetade också med testning under sprinten.

Jag deltog i **FE-38 – Undersök integrationstestning** och arbetade med **FE-39 – Konfigurera MSW** tillsammans med andra i gruppen.

Vi använde MSW för att simulera backend-svar så att frontend kunde testas utan att alla riktiga backend-tjänster behövde vara igång.

Jag arbetade med och körde tester med Vitest och React Testing Library.

Frontend hade fyra testfiler med totalt åtta tester, och samtliga tester passerade.

### Utmaningar och lösningar

En utmaning var att förstå vad gatewayen faktiskt gjorde mellan frontend och de olika mikrotjänsterna.

Genom att först skapa en egen gateway och sedan arbeta med den gemensamma gatewayen fick jag en mycket bättre förståelse för hur flödet fungerar.

Jag behövde också förstå skillnaden mellan att testa mot den riktiga backendmiljön och att använda MSW för att simulera API-svar.

Jag arbetade stegvis och använde testresultaten för att kontrollera att funktionerna fungerade som förväntat.

### Samarbete och agilt arbete

Gatewayuppgiften var ett bra exempel på hur vi arbetade gemensamt med lärande.

Alla fick först prova att skapa en egen lösning. Därefter jämförde vi våra lösningar och valde en gemensam gateway som hela gruppen kunde använda.

Vi hjälptes också åt med MSW och integrationstestningen och delade kunskap mellan oss.

Under våra dagliga avstämningar tog vi upp problem med gatewayen och mikrotjänsterna så att ingen skulle bli blockerad.

---

## Sprint 6 – vecka 44

### Vad jag arbetade med

Under den sista sprinten arbetade jag mycket med auth-service, felsökning, deployment, dokumentation och förbättringar i frontend.

### Auth-service och deployment

Jag arbetade med att driftsätta auth-service på Render.

I produktionsmiljön skulle auth-service använda PostgreSQL, medan jag lokalt använde H2.

Jag konfigurerade environment variables och Spring-konfigurationen för PostgreSQL och testade att auth-service kunde ansluta korrekt.

Jag arbetade också med JWT och JWKS.

Jag testade endpointen `/auth/jwks`, som andra mikrotjänster använder för att verifiera JWT-token.

Jag arbetade även med `/auth/me`, som används för att kontrollera vem som är inloggad.

### Felsökning mellan mikrotjänster

Jag körde hela systemet lokalt och felsökte kommunikationen mellan auth-service, gateway, product-service och order-service.

Jag upptäckte bland annat problem med portar och konfiguration mellan tjänsterna.

Lokalt kördes:

- auth-service på port `8080`
- product-service på port `8081`
- order-service på port `8082`
- gateway på port `9003`
- frontend på port `5173`

Jag felsökte ett problem där product-service inte kunde verifiera JWT eftersom tjänsten inte kunde hämta JWKS från auth-service.

Jag testade `/auth/jwks` direkt för att kontrollera att auth-service fungerade och startade sedan om tjänsterna. Efter det fungerade kommunikationen igen.

Jag arbetade även med problem i orderflödet. Gatewayen gav först 404 och senare 500. Jag kontrollerade gatewayens endpoint, order-service och konfigurationen mellan order-service och product-service steg för steg.

### FE-43 – Skapa README-filer för systemets repositories

Jag ansvarade för README-filen för auth-service.

Jag dokumenterade bland annat:

- vad auth-service används till
- hur autentisering och JWT fungerar
- vilka tekniker som används
- hur tjänsten startas
- relevanta endpoints
- H2 för lokal utveckling
- PostgreSQL i produktionsmiljön
- kopplingen mellan auth-service och gateway

### FE-44 – Informera om nödvändiga cookies

Jag skapade en informationsbanner i frontend som informerar användaren om att webbshoppen använder en nödvändig cookie för inloggning.

Bannern förklarar att cookien behövs för att användaren ska kunna vara inloggad och att den inte används för marknadsföring.

Jag lade till en Stäng-knapp.

När användaren stänger bannern sparas:

`cookie-info-closed = true`

i `localStorage`.

Jag testade även funktionen i webbläsarens utvecklarverktyg för att kontrollera att värdet sparades korrekt och att bannern inte visades igen efter omladdning.

### FE-45 – Finputsning av frontendens design

Jag arbetade med mindre förbättringar av frontendens design.

Jag upptäckte att det fanns två Logga ut-knappar i gränssnittet och tog bort den duplicerade knappen.

Jag justerade också cookie-bannerns storlek och layout så att den blev mindre och mer diskret.

Ändringarna gjordes i egna branches och skickades genom pull requests.

### FE-46 – Dokumentera backend med Javadoc

Jag dokumenterade de viktigaste delarna av auth-service med Javadoc.

Jag lade till dokumentation i:

- `AuthController`
- `AuthService`
- `JwtService`

Dokumentationen beskriver vad klasserna och metoderna gör samt relevanta parametrar, returvärden och fel.

### Utmaningar och lösningar

En stor utmaning var att auth-service på Render först använde fel databaskonfiguration och inte PostgreSQL som tänkt.

Jag kontrollerade environment variables och Spring-konfigurationen tills loggarna visade att PostgreSQL användes korrekt.

Lokalt fick jag också problem med H2-databasen där tabeller försvann.

Jag kontrollerade local-profilen och justerade databaskonfigurationen så att den lokala miljön fungerade igen.

En annan utmaning var JWT-verifieringen mellan product-service och auth-service.

Genom att läsa loggarna kunde jag se att problemet handlade om JWKS. Jag testade endpointen separat och kunde sedan verifiera att kommunikationen fungerade.

Jag arbetade även med felsökning av orderflödet och kontrollerade varje del steg för steg för att hitta var felet låg.

### Samarbete och agilt arbete

Under den sista sprinten fokuserade vi mycket på att få alla delar av systemet att fungera tillsammans inför redovisningen.

När jag hittade problem i en tjänst som någon annan ansvarade för försökte jag först identifiera problemet och sedan informera den ansvariga personen istället för att ändra deras kod utan samordning.

Jag använde branches och pull requests för frontendändringarna eftersom `main` var skyddad.

Jag arbetade iterativt genom att göra en mindre ändring i taget, testa den och därefter committa eller skapa en pull request när funktionen fungerade.

Vi hjälptes åt att felsöka integrationen mellan tjänsterna och prioriterade det som behövde bli klart inför presentationen.

---

# Sammanfattning av vad jag har lärt mig

Under projektet har jag fått en mycket bättre förståelse för hur ett system med flera mikrotjänster fungerar.

Jag har lärt mig mer om:

- Spring Boot och mikrotjänster
- autentisering med JWT
- roller och behörighet
- JWKS och verifiering av JWT mellan tjänster
- H2 för lokal utveckling
- PostgreSQL i produktionsmiljö
- deployment på Render
- hur en gateway fungerar mellan frontend och backend
- React och kommunikation mellan frontend och backend
- cookies och `localStorage`
- integrationstestning med Vitest, React Testing Library och MSW
- Git, branches, commits och pull requests
- felsökning med loggar, DevTools och API-anrop
- hur externa betalningslösningar som Klarna och Swish kan undersökas inför en framtida integration

En av de viktigaste sakerna jag har lärt mig är att det inte räcker att varje mikrotjänst fungerar separat. Alla delar måste också kunna kommunicera korrekt med varandra för att hela systemet ska fungera.

Jag har också blivit bättre på felsökning. Istället för att ändra flera saker samtidigt har jag lärt mig att testa en del i taget, läsa loggar och stegvis hitta var ett problem ligger.

Projektet har dessutom gett mig en bättre förståelse för agilt arbete. Genom sprintplanering, dagliga avstämningar, sprint review och retro har jag lärt mig att planera mitt arbete, kommunicera problem tidigt och anpassa arbetet när något tar längre tid än förväntat.

Jag har även fått erfarenhet av att samarbeta i ett projekt där olika personer ansvarar för olika delar. När ett problem har legat i en annan mikrotjänst har jag lärt mig att kommunicera med den ansvariga personen och samarbeta kring lösningen istället för att göra ändringar utan samordning.
