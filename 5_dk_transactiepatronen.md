# Transactiepatronen in Digikoppeling

In dit hoofdstuk beschrijven we de transactiepatronen in gegevensuitwisseling in algemene zin, met een suggestie welk Digikoppeling koppelvlakstandaard hier het best bij aansluit. Voor het opstellen van de volgende transactiepatronen is dankbaar gebruik gemaakt van de conceptversie van de *Edukoppeling Architectuur 2.0*.  


### Synchrone bevraging

Bij een bevraging (vraag-antwoord) stuurt de service-requester een voorgedefinieerde vraag (request) aan de service-provider, die een antwoord (response) verstrekt. Het initiatief ligt bij de service-requester. Gaat er in de uitwisseling iets mis dan zal de service-requester na een bepaalde tijd de uitwisseling afbreken (time-out). Een synchrone bevraging is in de regel *idempotent*, een request kan opnieuw verstuurd worden zonder gevolgen. 

![Synchroon Request](media/Synchroon_request.png "Synchroon Request")


|Koppelvlakspecificatie|Omschrijving|Praktijkvoorbeeld|
|---|---|---|
|Digikoppeling WUS| Digikoppeling WUS is geschikt als voor de bevraging gestructureerde  berichten (in XML) nodig zijn. Digikoppeling heeft profielen voor signing en encryption. |...|
|Digikoppeling REST API| Digikoppeling REST API heeft een GET methode waarmee synchrone requests kunnen uitgevoerd. Digikoppeling REST API kent nog geen gestandaardiseerde versies voor signing of encryptie| Bevragen OIN register via de COR API |</span>


Tabel 5.1: Synchrone bevraging

### Synchrone Melding

Bij een melding-bevestiging stuurt een service-requester informatie naar de service-provider en de ontvangst wordt synchroon door de service-provider bevestigd. Belangrijk is de schadelijke effecten te voorkomen als een bericht twee keer wordt verzonden (door een time-out) of als meldingen in de verkeerde volgorde binnenkomen.


|Koppelvlakspecificatie|Omschrijving|Praktijkvoorbeeld|
|---|---|---|
|Digikoppeling WUS| Digikoppeling WUS is geschikt als voor de melding een gestructureerde bericht (in XML) nodig is. Digikoppeling heeft profielen voor signing en encryption. Voorwaarde is dat de melding *idempotent* is |...|
|Digikoppeling REST API| Digikoppeling REST API heeft een PUT methode waarmee synchrone requests kunnen uitgevoerd. Digikoppeling REST API kent nog geen gestandaardiseerde versies voor signing of encryptie Het Digikoppeling REST API profiel kent ook een POST methode. POST is niet idempotent en kan dus niet herhaaldelijk worden verzonden| Binen Haal-Centraal kan een nieuwe resource worden gecreeerd in de Basisadministratie zoals de BAG of de BRP |

Tabel 5.2: Synchrone Melding

### Asynchrone Melding-bevestiging

Bij een melding-bevestiging stuurt een service-requester informatie naar de service-provider en ontvangt synchroon een bevestiging dat een bericht is ontvangen. op een later moment kan de ontvanger een bericht sturen dat de melding is verwerkt.  

![Asynchroon Request](media/Asynchroon_request.png "Asynchroon Request")


|Koppelvlakspecificatie|Omschrijving|Praktijkvoorbeeld|
|---|---|---|
|Digikoppeling ebMS2| Digikoppeling ebMS heeft reliable profiel (osb-rm) dat de bevestiging van ontvangst borgt | formele overdracht van OLO/DSO naar bevoegd gezag |
|Digikoppeling WUS| Digikoppeling WUS kent geen reliable profiel. Partijen in de keten moeten met elkaar afspraken hoe een melding wordt bevestigd in een antwoord door de ontvanger op een later tijdstip  |...|
|Digikoppeling REST API| Digikoppeling REST API heeft een PUT en een POST methode waarmee synchrone requests kunnen uitgevoerd. Digikoppeling REST API kent geen reliable profiel. Partijen in de keten moeten met elkaar afspraken hoe een melding wordt bevestigd in een antwoord door de ontvanger op een later tijdstip. Eventueel als onderdeel van een conversatie op business niveau | Door middel van de PUT methode kan een nieuw bedrijfsadres worden opgegeven bij de KVK API en d.m.v. POST kan het bedrijf worden genotificeerd over de status van de verhuismelding |

Tabel 5.3: Asynchrone Melding-bevestiging

### Uitwisselen grote bestanden

De situatie kan zich voordoen dat een bericht een omvang krijgt die niet meer efficiënt door de Digikoppeling-adapters verwerkt kan worden bijvoorbeeld vanwege de overhead bij eventuele hertransmissies. Ook kan het voorkomen dat er behoefte bestaat aan het sturen van aanvullende informatie naar systemen buiten de normale procesgang ('out-of-band').


|Koppelvlakspecificatie|Omschrijving|Praktijkvoorbeeld|
|---|---|---|
|Digikoppeling Grote berichten| Bij ‘grote berichten’ worden grotere bestanden uitgewisseld via een van de Digikoppelingkoppelvlakken in combinatie met een (HTTPS-)download vanaf een beveiligde website. Grote berichten vormen een functionele uitbreiding op de Digikoppelvlakstandaarden voor de veilige bestandsoverdracht van berichten groter dan 20 MiB | Decentrale overheden uploaden hun archief bestanden bij de grote berichten service van het Nationaal archief en dragen via een Digikoppeling koppelvlak de verantwoordelijkheid voor de archiefstukken over |

Tabel 5.4: Uitwisselen grote bestanden

### Uitwisseling via een transparante intermediair

Een transparante keten is alleen mogelijk als zowel de service-aanbieder als de serviceafnemer hetzelfde protocol hanteren. De intermediair routeert berichten tussen de serviceaanbieder en de serviceafnemer waarbij het bericht intact blijft (alleen de header wordt gelezen). De uitwisseling verloopt op dezelfde manier als bij een bilaterale uitwisseling.

![Transparante Intermediair](media/transparante_intermediair.png "Transparante Intermediair")


|Koppelvlakspecificatie|Omschrijving|Praktijkvoorbeeld|
|---|---|---|
|Digikoppeling WUS | Gebruik Digikoppeling WUS header voor routering  | ... |
|Digikoppeling ebMS | Gebruik Digikoppeling ebMS header voor routering| ... |</span>

Tabel 5.5: Transparante intermediair

### Uitwisseling via een niet-transparante intermediair

Een transparante keten is alleen mogelijk als zowel de service-aanbieder als de serviceafnemer hetzelfde protocol hanteren. De intermediair routeert berichten tussen de serviceaanbieder en de serviceafnemer waarbij het bericht bewerkt moet worden voor verdere verzending. 

![Niet-Transparante Intermediair](media/niet_transparante_intermediair.png "Niet-Transparante Intermediair")


|Koppelvlakspecificatie|Omschrijving|Praktijkvoorbeeld|
|---|---|---|
|Digikoppeling WUS |Gebruik Digikoppeling WUS header voor routering| ... |
|Digikoppeling ebMS |Gebruik Digikoppeling ebMS header voor routering| ... |</span>

Tabel 5.5: Niet-Transparante intermediair
