# Bijlage C: NORA Architectuurprincipes

Onderstaand wordt de relatie tussen NORA algemene principes en Digikoppeling principes aangegeven.
Zie [NORA Architectuur afspraken (2023)](https://www.noraonline.nl/wiki/Bindende_Architectuurafspraken)

## Architectuurprincipes

De architectuurprincipes geven richting aan de Digikoppeling-standaarden en Digikoppeling-voorzieningen en zijn afgeleid van de NORA Principes (zie bijlage C):

1. **Interoperabiliteit:** De interoperabiliteit van diensten is mogelijk door het gebruik van bewezen interoperabele internationale standaarden.

2. **Standaardoplossingen:** Het gebruik van standaardoplossingen is mogelijk, met een minimum aan ontwikkelinspanning of maatwerk.

3. **Veiligheid en vertrouwelijkheid:** Gegevens worden veilig uitgewisseld conform de eisen van de toepasselijke wet en regelgeving. Wanneer berichten met persoonsgegevens verstuurd worden, moeten serviceaanbieder en serviceafnemer nagaan of de uitwisseling voldoet aan de wet- en regelgeving (in het bijzonder de AVG).

4. **Betrouwbaarheid:**  Berichtaflevering is betrouwbaar indien nodig.

5. **Ontkoppeling:** De ontkoppeling van diensten wordt mogelijk door de verantwoordelijkheid van de logistieke laag, de transportlaag en de bedrijfsproceslaag strikt te scheiden.

## Relatie NORA Principes - Digikoppeling Principes 

| [ID](https://www.noraonline.nl/wiki/Eigenschap:ID "Eigenschap:ID") | Naam                                                                                                                                                                                                                                                                             | [Niveau afspraak](https://www.noraonline.nl/wiki/Eigenschap:Elementtype "Eigenschap:Elementtype")  | Digikoppeling Principe | Toelichting Relatie                                                                                               |
| ------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | --------------------- | ----------------------------------------------------------------------------------------------------------------- |
| NAP01                                                              | [Verplaats je in de gebruiker](https://www.noraonline.nl/wiki/Verplaats_je_in_de_gebruiker "Verplaats je in de gebruiker")                                                                                                                                                       | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP02                                                              | [Geef inzicht in de afhandeling van de dienst](https://www.noraonline.nl/wiki/Geef_inzicht_in_de_afhandeling_van_de_dienst "Geef inzicht in de afhandeling van de dienst")                                                                                                       | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP03                                                              | [Lever een kanaal-onafhankelijk resultaat](https://www.noraonline.nl/wiki/Lever_een_kanaal-onafhankelijk_resultaat "Lever een kanaal-onafhankelijk resultaat")                                                                                                                   | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP04                                                              | [Bundel diensten](https://www.noraonline.nl/wiki/Bundel_diensten "Bundel diensten")                                                                                                                                                                                              | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP05                                                              | [Bied de dienst proactief aan](https://www.noraonline.nl/wiki/Bied_de_dienst_proactief_aan "Bied de dienst proactief aan")                                                                                                                                                       | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP06                                                              | [Hergebruik vóór kopen vóór maken](https://www.noraonline.nl/wiki/Hergebruik_v%C3%B3%C3%B3r_kopen_v%C3%B3%C3%B3r_maken "Hergebruik vóór kopen vóór maken")                                                                                                                       | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Interoperabiliteit    | Digikoppeling koppelvlakstandaarden ondersteunen hergebruik van diensten                                                                |
| NAP07                                                              | [Bouw diensten modulair op](https://www.noraonline.nl/wiki/Bouw_diensten_modulair_op "Bouw diensten modulair op")                                                                                                                                                                | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Ontkoppeling          | Digkoppeling ondersteunt modulaire opbouw / architectuur                                                        |
| NAP08                                                              | [Standaardiseer waar mogelijk](https://www.noraonline.nl/wiki/Standaardiseer_waar_mogelijk "Standaardiseer waar mogelijk")                                                                                                                                                       | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Interoperabiliteit    | Digikopeling standaardiseert koppelvlakken                                                                                                                   |
| NAP09                                                              | [Beschrijf de dienst nauwkeurig](https://www.noraonline.nl/wiki/Beschrijf_de_dienst_nauwkeurig "Beschrijf de dienst nauwkeurig")                                                                                                                                                 | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP10                                                              | [Neem gegevens als fundament](https://www.noraonline.nl/wiki/Neem_gegevens_als_fundament "Neem gegevens als fundament")                                                                                                                                                          | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Ja                    | (REST) API's ondersteunen specifiek operaties op een data resource                                                |
| NAP11                                                              | [Pas doelbinding toe](https://www.noraonline.nl/wiki/Pas_doelbinding_toe "Pas doelbinding toe")                                                                                                                                                                                  | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP12                                                              | [Informeer bij de bron](https://www.noraonline.nl/wiki/Informeer_bij_de_bron "Informeer bij de bron")                                                                                                                                                                            | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Ja                    | (REST) API's ondersteunen specifiek operaties op een data resource                                                |
| NAP13                                                              | [Beheers risico's voortdurend](https://www.noraonline.nl/wiki/Beheers_risico%27s_voortdurend "Beheers risico's voortdurend")                                                                                                                                                     | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP14                                                              | [Verifieer altijd](https://www.noraonline.nl/wiki/Verifieer_altijd "Verifieer altijd")                                                                                                                                                                                           | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| NAP15                                                              | [Maak diensten schaalbaar](https://www.noraonline.nl/wiki/Maak_diensten_schaalbaar "Maak diensten schaalbaar")                                                                                                                                                                   | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Ja                    | API concepten ondersteunen modulaire opbouw / architectuur (en daarmee een schaalbare opzet)                      |
| NAP16                                                              | [Voorkom onnodige complexiteit](https://www.noraonline.nl/wiki/Voorkom_onnodige_complexiteit "Voorkom onnodige complexiteit")                                                                                                                                                    | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") | Ja                    | API kunnen complexiteit verminderen (door modulaire opbouw en door complexiteit te verbergen achter de interface) |
| NAP17                                                              | [Stuur cyclisch op kwaliteit](https://www.noraonline.nl/wiki/Stuur_cyclisch_op_kwaliteit "Stuur cyclisch op kwaliteit")                                                                                                                                                          | [Architectuurprincipe](https://www.noraonline.nl/wiki/Architectuurprincipe "Architectuurprincipe") |                       |                                                                                                                   |
| | | | | | 



OUD
**TODO: helemaal vervangen door nieuwe [NORA afsrpaken](https://www.noraonline.nl/wiki/Bindende_Architectuurafspraken)**

De NORA (Nederlandse Overheids Referentie Architectuur) is de bron voor de architectuur principes. NORA definieert 10 basisprincipes<sup>[34](#f34)</sup>
<br>
<sup><a name="f34"><dfn>34</dfn></a>:  *Bron: [https://www.noraonline.nl/wiki/Principes](https://www.noraonline.nl/wiki/Principes)*</sup>

Overzicht


| Principe      | Statement                                                                                      | ID   |
|---------------|------------------------------------------------------------------------------------------------|------|
| PROACTIEF     | Afnemers krijgen de dienstverlening waar ze behoefte aan hebben.                               | BP01 |
| VINDBAAR      | Afnemers kunnen de dienst eenvoudig vinden.                                                    | BP02 |
| TOEGANKELIJK  | Afnemers hebben eenvoudig toegang tot de dienst.                                               | BP03 |
| STANDAARD     | Afnemers ervaren uniformiteit in de dienstverlening door het gebruik van standaardoplossingen. | BP04 |
| GEBUNDELD     | Afnemers krijgen gerelateerde diensten gebundeld aangeboden.                                   | BP05 |
| TRANSPARANT   | Afnemers hebben inzage in voor hen relevante informatie.                                       | BP06 |
| NOODZAKELIJK  | Afnemers worden niet geconfronteerd met overbodige vragen.                                     | BP07 |
| VERTROUWELIJK | Afnemers kunnen erop vertrouwen dat informatie niet wordt misbruikt.                           | BP08 |
| BETROUWBAAR   | Afnemers kunnen erop vertrouwen dat de dienstverlener zich aan afspraken houdt.                | BP09 |
| ONTVANKELIJK  | Afnemers kunnen input leveren over de dienstverlening.                                         | BP10 |

zie ook [https://www.noraonline.nl/wiki/Basisprincipes_totaaloverzicht](https://www.noraonline.nl/wiki/Basisprincipes_totaaloverzicht)

Tabel 12.1: NORA Basisprincipes

| NORA Afgeleide principes | ID | Stelling | Cluster | Realiseert | DK principes |
|---|---|---|---|---|---|
| Diensten zijn herbruikbaar                 | AP01 | De dienst is zodanig opgezet dat andere organisaties deze in eigen diensten kunnen hergebruiken. | Diensten-aanbod | Standaard (Basisprincipe) | DK 1. interoperabiliteit |
| Ontkoppelen met diensten                   | AP02 | De stappen uit het dienstverleningsproces zijn ontsloten als dienst. | Diensten-aanbod | Noodzakelijk | DK 5: Digikoppeling maakt ontkoppeling mogelijk. |
| Nauwkeurige dienst-beschrijving            | AP05 | De dienst is nauwkeurig beschreven. | Diensten-aanbod | Transparant<br>Vindbaar | DK is open en beschreven in de architectuur en koppelvlakstandaarden. |
| Gebruik standaard oplossingen              | AP06 | De dienst maakt gebruik van standaard oplossingen | Standaard oplossingen | Standaard (Basisprincipe) | DK 2. Standaard oplossingen |
| Gebruik de landelijke bouwstenen           | AP07 | De dienst maakt gebruik van de landelijke bouwstenen e-overheid | Standaard oplossingen | Standaard (Basisprincipe) | DK 2. Standaard oplossingen |
| Gebruik open standaarden                   | AP08 | De dienst maakt gebruik van open standaarden | Standaard oplossingen | Standaard (Basisprincipe) | DK 1. interoperabiliteit |
| Voorkeurskanaal internet                   | AP09 | De dienst kan via internet worden aangevraagd | Kanalen | Toegankelijk | DK 1. interoperabiliteit |
| Informatie-objecten systematisch beschreven| AP17 | De aan de dienst gerelateerde informatieobjecten zijn, uniek geïdentificeerd, in een informatiemodel beschreven. | Informatie | Vindbaar<br>Toegankelijk<standaard> | DK 3. Veiligheid en vertrouwelijkheid |
| Afspraken vastgelegd                       | AP28 | Dienstverlener en afnemer hebben afspraken vastgelegd over de levering van de dienst | Sturing en verantwoordelijkheid | Betrouwbaar | DK 4. Betrouwbaarheid |
| De dienst-verlener voldoet aan de norm     | AP29 | De dienstverlener draagt zelf de consequenties wanneer de dienst afwijkt van afspraken en standaarden. | Sturing en verantwoordelijkheid | Standaard (Basisprincipe)<br>Betrouwbaar | DK 1. interoperabiliteit |
| Uitwisseling berichten onweerlegbaar       | AP40 | De berichtenuitwisseling is onweerlegbaar | Betrouwbaarheid | Betrouwbaar | DK 4. Betrouwbaarheid |
| Beschikbaarheid                            | AP41 | De beschikbaarheid van de dienst voldoet aan de met de afnemer gemaakte continuïteitsafspraken. | Betrouwbaarheid | Betrouwbaar | DK 4. Betrouwbaarheid |
| Vertrouwelijkheid (principe)               | AP43 | De dienstverlener zorgt ervoor dat de beoogde toegang tot gegevens en de juiste werking van zijn systemen continu alsook achteraf te controleren is. | Betrouwbaarheid | Betrouwbaar<br>Vertrouwelijk | DK 3. Veiligheid en vertrouwelijkheid |

Tabel 12.2: Relevante afgeleide NORA principes en mapping naar Digikoppeling (DK) principes
zie [https://www.noraonline.nl/wiki/Afgeleide_principes_tabel](https://www.noraonline.nl/wiki/Afgeleide_principes_tabel)
