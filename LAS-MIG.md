# RenoveringsByggarna – ny webbplats

Färdiga statiska HTML-filer finns i `dist/`. Ingen installation, databas eller byggprocess behövs för att använda dem.

## Innehåll
- Startsida med fullbreddshero och företagets ursprungliga blå logotyp.
- Kök, badrum, övrig renovering, produkter/material, referenser, om oss, kontakt, integritet och felsida.
- Samtliga 66 referensbilder från originalets galleri finns lokalt i WebP. Bilder kan filtreras och öppnas i sin helhet.
- Telefon- och mejllänkar. På mobilen visas en fast kontaktlist.
- Inga formulär som låtsas skicka, ingen webbshop och ingen spårningskod.
- Unika titlar, beskrivningar, canonical, sociala förhandsvisningar, företagsdata, brödsmulor, sitemap och robots.txt.

## Källor kontrollerade 17 november 2026
Företagets egna sidor: http://renoveringsbyggarna.se/hem, /om-oss, /produkter-o-tjanster, /referenser och /kontakt.
Logo, startbild och alla referensbilder kommer från dessa sidor. Inga nya AI-projektbilder eller påhittade kundcitat används.

Google Maps: https://www.google.com/maps?cid=4621940237449796760
Det verifierade betyget är **3,0/5 från 2 omdömen**, kontrollerat i den synliga Google-profilen. Kataloguppgiften 5,0/1 är inaktuell. På kundens begäran visas inget betyg, inga stjärnor och inget antal på webbplatsen. Omdömessektionen länkar till samtliga originalomdömen på Google. Ingen automatisk Google-widget eller påhittade citat används.

## Publicering
Ladda upp innehållet i `dist` till webbhotellets dokumentrot, eller till roten i ett GitHub Pages-repository. Behåll mappen `assets` och alla HTML-, CSS- och JavaScript-filer. Enbart index.html räcker inte.

I Sites-versionen pekar canonical, sitemap och sociala metadata på designens förhandsvisningsadress. GitHub/webbhotell-paketet har dessa adresser ändrade till företagets nuvarande domän http://renoveringsbyggarna.se. När HTTPS aktiverats, ändra denna basadress till https://renoveringsbyggarna.se i alla HTML-filer, sitemap.xml och robots.txt. Om ett annat domännamn ska indexeras, använd det i stället.

`.htaccess` innehåller omdirigeringar från originalets /hem, /om-oss, /produkter-o-tjanster, /referenser och /kontakt på Apache-kompatibla webbhotell, samt cache- och komprimeringsinställningar. GitHub Pages använder inte .htaccess. Aktivera HTTPS via webbhotellet. Skicka sitemap.xml till Google Search Console efter publicering på den riktiga domänen. Ingen ranking kan garanteras.

## Kontroll
Kontrollerat i webbläsaren på 320, 390 och 1440 px: ingen horisontell överströmning på tjänster, material, referenser, om oss eller kontakt; fungerande meny, FAQ, galleri, filter, visa fler, nästa bild och stängning. Kontrollerade telefon/mejl-adresser utan att ringa eller skicka meddelanden. Alla interna filreferenser, ankarlänkar, JSON-LD och grundläggande SEO-fält validerade. Inga konsolfel under granskningen.

`build.py` genererar HTML-filerna. Filerna i dist kan också redigeras direkt. `SITE_URL` kan användas för att generera med en annan basadress. `check-site.py` kontrollerar sidor och interna länkar.
