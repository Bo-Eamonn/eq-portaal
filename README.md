# PLannings Document!
In deze readme staan de pagina's en functionaliteiten welke gemaakt worden. In loop der tijd zal dit document ook bijgewerkt worden. Eventuele op/aan -merkingen zijn er altijd. Laten we dit dan ook zo goed mogelijk noteren.

> ### Streven
> Hier onder zijn een aantal strevens, soort sprints, soort doelstelling. Het gaat er eigenlijk om dat dat we een idee hebben wat wanneer een beetje van toepassing is. Eventuele streven mogen erbij gezet worden. Eenmaal afgerond dan markeren we dit 
> 
> 1. 01/09/2023 Front-end Volledig af 
> Dit houd in dat de layout af is,
> Alle pagina's gevult zijn met hardcoded dummydata,
> ClientSide Functionaliteiten werken,
> Functionaliteiten goed opgeschreven staan en ready zijn om ontwikkeld te worden.
> 2. 01/10/2023 Back-end Volledig af
> Dit houd in dat alle besproken functies werkend in de applicatie zitten.
> 3. 02/10/2023 - 31/12/2023 afwikkelingsfase
> Alles nalopen, testen, puntjes op de 'i' zetten. Fallbacks maken en testen. 

## Portaal
Beschrijvingen van Layout's, kleuren, inhoud en functionaliteit.
### Inloggen
Alles groter dan een tablet krijgt een "split" screen. Met rechts de mogelijkheid om in te loggen en links een het logo.
Kleiner dan een tablet wordt het gewoon het volledige scherm. Anders is het ook niet aanklikbaar.

Het daadwerkelijke inlog form met een ronde/zachte afwerking

Qua kleuren eigenlijk de kleuren te gebruiken vanuit het logo, Dan krijg je Blauw, Geel, Wit en Zwart. Hier verschillende tinten van te gebruiken.

### Home
De home page bestaat bestaat uit 3 delen
1. NAV/Aside
Rechts van het scherm hebben we de navigatie. Vanuit hier kan de klant kiezen wat er in de main weergegeven word.
Onderaan de nav is een optie om van _light_ naar _dark_ theme te switchen.
2. Main>Section
De ruimte die nu op de pagina leeg is, is de main. Hierin worden de pagina's weergegeven worden welk vanuit de nav opgevraagd worden.

*Personeel*

Het personeel ziet natuurlijk andere dingen dan wat een klant te zien krijgt. 
Hieronder staan de menu opties:
*  Home
* Zendesk (new tab)
* Saysimple (new Tab)
* Klanten
* Voorraad
* Kennisbank
> Personeel ziet op de homepage de zelfde opties als in het menu. Eventueel later nog mogelijk te maken dit te customizen

*Klanten*

Klanten zien daar in tegen natuurlijk weer andere dingen.
Hieronder staan de menu opties:
* Home
* Gegevens
* Contact
* Kennisbank
> Klanten krijgen 2 verschillende homepages.
> 1. Het scherm om het wachtwoord aan te passen zodra ze voor het eerst inloggen
> 2. Algemeen scherm met huidige statusen. Denk aan algemene storingen, statussen en zendingen.
### Klanten
De klanten pagina is alleen zichtbaar voor het personeel. Hier in kan het personeel een klant zoeken, aanpassen en toevoegen.
Voor het toevoegen en bewerken openen er nieuwe schermen (Modals, sort pop-up)
> #### Toevoegen
> Bij het toevoegen van een nieuwe klant vullen we de naam, onderneming & contact gegevens in. Dan krijgt de klant automatisch een mail om het profiel af te ronden. 
>  ***
>  Ook wordt er bij het aanmaken aangegeven om welke set het gaat en welke hardware hiervoor gebruikt gaat worden. Dit word dan automatisch uit de beschikbare voorraad gekoppeld aan de nieuwe klant.

> #### Bewerken/aanpassen
> Hier kan het personeel statussen aanpassen, gegevens aanpassen en de inlog mail opnieuw sturen. Met natuurlijk een nieuwe klant toevoegen.
> De aanpasbare gegevens zijn;
> - Naam van de klant
> - Naam van de onderneming
> - e-mail 
> - Telefoonnummer 
> - Adres


### Voorraad
Voorraad is een andere pagina die alleen door het personeel zichtbaar is. Hier kunnen we de voorraad van inzien. Standaard zien we eigenlijk de aantallen van wat er nu beschikbaar is.
De de voorraad welke wij zien zijn;
1. De POS systemen (met werkende klantenscherm)
2. Kassa lades
3. Bon printers
4. Barcode handscanners
5. Barcode Blokscanners
6. Megallan weegschaal/scanner combinaties
7. Pinautomaten
8. Beschikbare POI's 
9. Beschikbare BS nummers
10. handhelds 

Per elke soort voorraad hebben we een kleine box waar wij op geklikt kan worden, zodat we het overzicht kunnen zien. In de box zelf zien we naast de naam ook het aantal beschikbaar.
Op de voorraad pagina van het soort, kunnen we nieuwe voorraad toevoegen, voorraad verwijderen en de status/klant aanpassen.
Naast het toepassen van CRUD kunnen we ook de weergave aanpassen. Denk aan sorteren op basisis van status en/of datum
### Gegevens
Gegevens is de pagina voor de klant. Hier heeft de klant een overzicht van de bij ons bekend/aangeleverde gegevens. De eerste keer dat ze deze pagina bezoeken word gevraagd de gegevens te controleren en eventueel bijwerken / aanleveren.
Dit zijn gegevens die zichtbaar zijn voor de klant welke sommige door de klant aangepast kunnen worden.
1. Naam onderneming\*
2. KvK nummer\*
3. Naam Klant\*
4. Contactgegevens\*
5. Sepay contract\**
6. Foto's binnen / buiten\**
7. ID eigena(a)r(en)\*
8. Productlijst/menukaart\**
9. Plattegrond\**
10. Afschrift\**
11. Sepay Klantnummer\***
12. EQPOS Klantnummer\***
13. Hardware ID's en/of POI/BS-nummers \***
 
Bij bijvoorbeeld een wijziging van het rekeningnummer kan de klant dit ook vanuit hier invullen. Dit omdat de overige gegevens hiervoor gekoppeld staan vanuit de voorraad met de klant. Eventuele aanvragen om Amex aan te zetten kan dan ook hier. Dit zal dan ook een status moeten triggeren dat het aangevraagd is wat dan door personeel doorgezet kan/moet worden. En dus de status veranderd op het moment van aanpassing.

> #### Legenda
> Gegevens met een \* zijn **verplicht**

> Gegevens met een \** zijn **optioneel**

> Gegevens met een \*** zijn **niet** aanpasbaar door de klant

 
### Contact
De contact pagina, spreekt enigszins voor zichzelf. Maar hier komen een X aantal belangrijke features. 
Het content scherm word hier dan ook in 4 delen gedeeld. een 1/3 verhouden. Horizontaal gescheiden. Met in de bovenste helft een stukje tekst. Een korte uitleg wanneer mensen niet of juist wel moeten bellen.
Dat ondanks een appje sturen makkelijk is, de beller sneller is. Wanneer een pinautomaat of de kassa het niet doet. Direct bellen.

Dan in de onderste helft hebben we 3 vakken verticaal gescheiden. Met natuurlijk wat informatie.
- Verkoop
09:00 - 17:00 
Ma t/m Vrij
3 icoontjes, een telefoon, het whatsapp logo en het e-mail icoontje.
Wanneer hier op geklikt word, wordt er automatisch doorgeschakeld naar de desbetreffende service.

- Support
09:00 - 17:00
Ma t/m Vrij 
Alle algemene vragen en storingen met betrekking tot het systeem
Buiten deze tijden kunt u voor algemene vragen en niet extreme storingen mailen of een whatsapp bericht sturen, dan word dit zo snel mogelijk opgepakt.
Bij Grote storingen (kassa die niet aan gaat, Pinautomaat wat niet werkt of als er rook uit de kassa komt) Altijd direct bellen. 
3 icoontjes, een telefoon, het whatsapp logo en het e-mail icoontje.
Wanneer hier op geklikt word, wordt er automatisch doorgeschakeld naar de desbetreffende service.

- Administratie
09:00 - 17:00 
Ma t/m Vrij
3 icoontjes, een telefoon, het whatsapp logo en het e-mail icoontje.
Wanneer hier op geklikt word, wordt er automatisch doorgeschakeld naar de desbetreffende service.
 
>Code blokken
>```html
><a href="tel:0850071077,1">Verkoop Direct Bellen</a>
><a href="tel:0850071077,2">Support Direct Bellen</a>
><a href="tel:0850071077,3">Administratie Direct Bellen</a>
>``` 
>
> Voor de whatsapp is het een ander verhaal. We kunnen 2 dingen doen namelijk
> 1. Dit is niks meer dan een nieuwe chat openen.
> Dit is ook de meest makkelijke optie.
> ```HTML
> <a href="https://wa.me/+31850071077" target="_BLANK">Whatsapp</a>
> ```
> 2.  Op onderstaande manier is het mogelijk om een berichtje alvast voor te schrijven.
> Onderstaande manier heeft als output "Goedendag ik zou graag in contact willen komen met iemand van de verkoop afdeling". Eventueel, kunnen we zelfs klant gegevens hierin verwerken, denk aan een naam of een klant nummer.
>```HTML
><a href="https://wa.me/+31850071077?text=Goedendag%20ik%20zou%20graag%20in%20contact%20willen%20komen%20met%20iemand%20van%20de%20verkoop%20afdeling." target="_BLANK">Whatsapp<a>
>```
 
### Kennisbank
Bij de kennisbank komen we weer op het punt dat dit gebruikt kan worden door zowel personeel als door klanten. Hier zit natuurlijk wel verschil in. De manier hoe dit mij logisch leek te doen is door de Zendesk API te gebruiken. Dan kunnen we Zendesk Guide koppelen aan het portaal. Afhankelijk van de API instellingen kan een onderscheid gemaakt worden tussen wat wel en niet zichtbaar is voor de klant en het personeel.

De API ziet er ongeveer zo uit, it is om alle artikelen te laten zien.
```https://eqposnl.zendesk.com/api/v2/help_center/en-us/articles.json```
Voor klanten kunnen we gebruik maken van categorieën;
```https://eqposnl.zendesk.com/api/v2/help_center/categories/{$helpCenterId}/articles.json```

>Zendesk Guide API documentatie
>https://developer.zendesk.com/api-reference/help_center/help-center-api/introduction/

*Personeel*

Personeel zal ten alle tijden alle artikelen in de kennisbank kunnen zien. Zo kan er telefonisch mee gekeken worden met wat de klant kan zien. Het grootse verschil is eigenlijk dat personeel ook stappenplannen en dergelijk kan terug vinden. Denk dan aan Storingen verhelpen op een manier wat niet toegankelijk is voor een klant. Of juist even terug zoeken hoe het portaal werkt.

*Klanten*

Omdat er langzamerhand steeds meer vraag komt vanuit klanten naar handleidingen. Standaard worden er uitleg video's verstuurd na de installatie. Omdat niet alle klanten de mogelijkheid hebben om dit te kijken en/of de video's wel eens kwijt geraakt worden door de klant. Is het fijn om 1 plek te hebben met zowel documentatie als met de video's.

Door geschreven documentatie te hebben in combinatie met video documentatie zal dit een groot probleem verhelpen. Daarnaast kunnen wij ook de standaard oplossingen verwerken. Printer uit en aan, internet controleren, kabels controleren etc etc.
