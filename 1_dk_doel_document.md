# Doel van dit document en leeswijzer

## Inleiding

Digikoppeling is een standaard voor gestructureerde gegevensuitwisseling waarmee overheden op een veilige manier gegevens met elkaar kunnen uitwisselen.

## Doel

De *Digikoppeling Architectuur* definieert de kaders – de gehanteerde principes en voorschriften - waarbinnen de gegevensuitwisseling op basis van Digikoppeling plaatsvindt en beschrijft de rol van intermediairs in de keten van gestructureerde gegevensuitwisseling.

## Doelgroep

De *Digikoppeling Architectuur* is bedoeld voor ICT-professionals in de publieke sector en voor ICT-leveranciers die Digikoppeling (willen gaan) gebruiken. Zie ook onderstaande tabel.

| Afkorting | Rol | Taak  | Doelgroep? |
| --------- | --- | --- | ------------ |
| [M]       | Management                      | Bevoegdheid om namens organisatie (strategische) besluiten te nemen.                                      | Nee    |
| [P]       | Projectleiding                  | Verzorgen van de aansturing van projecten.                                                                | Nee    |
| [A&D]     | Analyseren & ontwerpen (design) | Analyseren en ontwerpen van oplossings-richtingen. Het verbinden van Business aan de IT.                  | Ja     |
| [OT&B]    | Ontwikkelen, testen en beheer   | Ontwikkelt, bouwt en configureert de techniek conform specificaties. Zorgen voor beheer na ingebruikname. | Ja     |

Tabel 1.1: Doelgroep Digikoppeling Architectuur 

## Historie

De *Digikoppeling Architectuur* is tot stand gekomen in samenwerking met leden van het Technisch Overleg Digikoppeling en andere belanghebbenden.

De *Digikoppeling Architectuur* is mede gebaseerd op:

- De *Digikoppeling-koppelvlakstandaarden.* Onderdelen uit deze documenten zijn hier samengevat om voor de lezer duidelijk te maken.

- Het hoofdstuk over *de Digikoppeling keten* bevat elementen uit [*De Architectuurschets*](https://www.earonline.nl/index.php/Overzicht_Architectuurschets_van_het_stelsel_voor_gegevensuitwisseling), de context voor gegevensuitwisseling binnen de overheid in algemene zin en voor Digikoppeling in het bijzonder. *De Architectuurschets* is een  verouderd product uit 2012; de essentiële elementen van *De Architectuurschets* zijn gaandeweg ook opgenomen in de NORA en met name het het [*NORA Katern Verbinden*](https://www.noraonline.nl/wiki/Katern_Verbinden).

## Samenhang

De architectuur van Digikoppeling wordt regelmatig geactualiseerd om goed te blijven aansluiten op de behoeften van overheden en de wensen van de maatschappij. Actuele ontwikkelingen waarmee de Architectuur in 2024 in lijn wordt gebracht zijn onder andere:

- [De Interbestuurlijke Datastrategie (IBDS),](https://realisatieibds.pleio.nl/)
- [Het Federatief Datastelsel (FDS),](https://www.noraonline.nl/wiki/FDS_Basis_concept)
- [De Generieke Digitale Infrastructuur (GDI),](https://pgdi.nl/)
- [De Architectuur van het Kennisplatform API's,](https://geonovum.github.io/KP-APIs/API-strategie-algemeen/Architectuur/)
- De ontwikkelingen vanuit [Data bij de Bron](https://www.digitaleoverheid.nl/data-bij-de-bron/) en [Common Ground](https://commonground.nl/).

## Digikoppeling standaarden

De *Architectuur Digikoppeling* is onderdeel van de Digikoppeling-standaarden.
De documentatie is als volgt opgebouwd:

![Overzicht van de onderdelen van de Digikoppeling Standaard, de standaard is onderverdeeld in normatieve en ondersteunende onderdelen](media/DK_Specificatie_structuur.svg "Digikoppeling Standaard")

<details>
    <summary> Tekstalternatief </summary>
<ul>
	<li>Digikoppeling Standaard
		<ul>
			<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/beheer/">DK Beheermodel en releasebeleid</a>* </li>
			<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/actueel/">DK Overzicht Actuele Documentatie en Compliance</a>* </li>
			<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/architectuur">DK Architectuur</a>*
				<ul>
					<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/idauth/">DK Identificatie en Authenticatie</a>*
						<ul>
							<li><i> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/gbachtcert/">Digikoppeling Gebruik en Achtergronden Certificaten</a></i>† </li>
						</ul>
					</li>
					<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/beveilig/">DK Beveiligingsstandaarden en voorschriften</a>* </li>
					<li>Koppelvlakstandaarden
						<ul>
							<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/wus/">DK Koppelvlakstandaard WUS</a>*
								<ul>
									<li><i><a href="https://gitdocumentatie.logius.nl/publicatie/dk/bpwus">Best-practice WUS</a></i>† </li>
								</ul>
							</li>
							<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/ebms/">DK Koppelvlakstandaard ebMS2</a>*
								<ul>
									<li> <i><a href="https://gitdocumentatie.logius.nl/publicatie/dk/bpebms">Best-practice ebMS2</a></i>† </li>
								</ul>
							</li>
							<li> <a href="https://gitdocumentatie.logius.nl/publicatie/dk/gb/">DK Koppelvlakstandaard Grote Berichten</a>*
								<ul>
									<li> <i><a href="https://gitdocumentatie.logius.nl/publicatie/dk/bpgb">Best-practice Grote Berichten</a></i>†</li>
								</ul>
							</li>
						</ul>
					</li>
				</ul>
			</li>
			<li>
    <i><a href="https://gitdocumentatie.logius.nl/publicatie/dk/watisdk/">Wat is Digikoppeling</a></i>†
  </li>
		</ul>
	</li>
</ul>
<p>* Normatief document</p>
<p>† Ondersteunend document</p>
</details>

- Alle groene documenten vallen onder het beheer zoals geformaliseerd in het [[[?DK-Beheermodel]]].

- Een overzicht van alle Digikoppeling documentatie is opgenomen in [[[#bronnen]]].

- Alle goedgekeurde documenten zijn te vinden op de website van Logius: [[[DK-Doc]]].

  (_Opmerking : De Best Practice REST API is in ontwikkeling_)

## Begrippen

Belangrijke begrippen en afkortingen zijn opgenomen in [[[#begrippenlijst]]].
