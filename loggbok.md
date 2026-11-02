# Individuell loggbok – Webbshop

## Första sammanfattningen

### Vad jag har arbetat med

Jag har främst arbetat med auth-servern i projektet. Jag har arbetat med autentisering, JWT, roller och kopplingen mellan auth-servern och gatewayn.

Jag har även arbetat med driftsättning av auth-servern på Render och konfigurerat PostgreSQL för produktionsmiljön. Lokalt har jag arbetat med H2-databas och en separat local-profil.

Jag har felsökt flera problem i integrationen mellan frontend, gateway och mikrotjänsterna. Bland annat har jag undersökt problem med inloggning, JWT-verifiering, JWKS och kommunikation mellan gateway, product-service och order-service.

Jag har också:
- uppdaterat README för auth-servern
- lagt till Javadoc i `AuthController`, `AuthService` och `JwtService`
- arbetat med frontend och tagit bort en duplicerad logga ut-knapp
- skapat en informationsbanner för nödvändiga cookies
- arbetat med branches, commits och pull requests i GitHub

### Eventuella problem och hur jag löste dem

Ett problem var att auth-servern först använde fel databasinställningar i Render. Jag felsökte environment variables och databaskonfigurationen tills tjänsten använde PostgreSQL korrekt.

Jag hade också problem lokalt med H2-databasen och saknade tabeller. Jag löste det genom att kontrollera local-profilen och databaskonfigurationen.

När product-service inte kunde verifiera JWT undersökte jag loggarna och såg att tjänsten inte kunde hämta JWKS från auth-servern. Efter att auth-servern fungerade och JWKS-endpointen kunde nås startade jag om tjänsterna och kommunikationen fungerade igen.

Jag har även löst Git-konflikter i `application-local.properties` och varit noga med att lokala konfigurationer inte ska följa med i commits när de bara gäller min utvecklingsmiljö.

### Samarbete och agilt arbete

Jag har arbetat utifrån gruppens backlog och tagit ansvar för uppgifter som rör auth-servern. När problem har berört andra mikrotjänster har jag kommunicerat med den person som ansvarar för respektive tjänst istället för att ändra deras delar utan samordning.

Jag har använt branches och pull requests för frontendändringar eftersom `main` är skyddad. Jag har även granskat vilka uppgifter som är färdiga innan de flyttas vidare i backloggen.

Jag har försökt arbeta iterativt genom att göra en mindre ändring i taget, testa lokalt och sedan committa eller skapa en pull request när funktionen har verifierats.
