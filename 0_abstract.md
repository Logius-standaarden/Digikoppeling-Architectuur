Digikoppeling (DK) is sinds 2007 in gebruik en steeds meer overheidsorganisaties zien het nut van het gebruik van deze standaard. Digikoppeling wordt daardoor steeds breder ingezet als logistieke standaard voor veilige gegevensuitwisseling tussen organisaties in de (semi-)publieke sector in Nederland. Digikoppeling is een essentiële bouwsteen van de elektronische overheid en geeft invulling aan de servicegerichte architectuur zoals NORA die voorschrijft.

Digikoppeling standaardiseert de uitwisseling van gegevens (services) tussen overheidsorganisaties. Door Digikoppeling kunnen zij eenvoudiger, veiliger, sneller en goedkoper elkaars gegevens gebruiken dan wanneer alle organisaties bilateraal afspraken zouden maken. Het belang en de omvang van gegevensuitwisselingen in de e-overheid neemt alleen maar toe. Digikoppeling is een onmisbare voorwaarde om die uitwisseling efficiënt uit te voeren.

Het [OBDO](https://archief29.sitearchief.nl/archives/sitearchief/20231030233509/www.digitaleoverheid.nl/nieuws/overheidsbrede-beleidsoverleg-digitale-overheid-obdo/) heeft Digikoppeling daarom op de [‘Pas toe of leg uit’-lijst](https://forumstandaardisatie.nl/open-standaarden/verplicht) geplaatst. Deze lijst betreft onder meer de uitwisseling met wettelijke landelijke basisadministraties en gegevensuitwisseling tussen sectoren (intersectoraal). Daarnaast wisselen organisaties onderling of in samenwerkingsverbanden gegevens uit in de dienstverlening aan burgers en bedrijven op basis van Digikoppeling.

De *Architectuur Digikoppeling* beschrijft de kaders, de principes en voorschriften, de koppelvlakstandaarden, voorzieningen en de keten waarin via Digikoppeling gegevens worden uitgewisseld (de Digikoppeling keten).

Digikoppeling is 'backwards compatible'\*. Partijen die Digikoppeling gebruiken, voldoen daardoor automatisch aan de nieuwste versie van Digikoppeling. De nieuwe functionaliteiten en profielen zijn dan echter niet beschikbaar. Voor het beheer van de Digikoppeling standaard en documenten wordt waar mogelijk [Semantic Versioning](https://semver.org/spec/v2.0.0.html) toegepast.

De aanleiding van de vernieuwing van dit document is tweeledig: in 2019 is een RFC ingediend over relatie van de Digikoppeling profielen met *bevragen en melden*. Daarnaast is in 2020 een Rest API profiel uitgewerkt en opgenomen in de Digikoppeling Standaard.

De belangrijkste wijzigingen in de nieuwe Digikoppeling Architectuur versie 2 zijn: 

- Geen onderscheid meer in 'WUS voor bevragingen' en 'ebMS voor meldingen'
- Toevoegen van een Digikoppeling REST API profiel, gebaseerd op de API Design Rules (uit de Nederlandse API Strategie)
- De Provider bepaalt welk koppelvlak - REST API, WUS of ebMS van toepassing is op de door haar geleverde dienst.

**De implicatie van deze wijzigingen is dat organisaties bij doorontwikkeling, en nieuwbouw van voorzieningen zelf de keuze kunnen maken welk van de profielen het beste past bij hun ambitie.**

\*(‘Backwards compatibiliteit’ geldt niet voor de security eisen, zie hiervoor de actuele versie van [[[DK-Beveiliging]]])
