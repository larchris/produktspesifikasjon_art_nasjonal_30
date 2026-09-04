### Datamodell

**Kilde:** [SOSI UML XMI-fil](https://sosi.geonorge.no/svn/SOSI/SOSI%20Del%203/Miljodirektoratet/ArterNasjonalForvaltningsinteresse_3_0.xml)

<a href="ny-datakilde_feature_catalogue.png" title="Klikk for stor visning"><img src="ny-datakilde_feature_catalogue.png" alt="Datamodell Ny datakilde" style="max-width: 100%; height: auto;" /></a>

#### ArtForvaltningsinteresse

Forekomster/observasjoner av et kriteriebasert utvalg arter som er spesielt viktig for biologisk mangfold, samt fremmede arter som er en trussel mot naturlig biologisk mangfold. Alt innhold hentes fra Artsdatabankens infrastruktur, basert på arten og nærmere definerte tekniske kvalitetskriterier (geografisk presisjon mv.).

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>datoFra</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Startdato for registreringen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>datoTil</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Sluttdato for registreringen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>geografiskPresisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angis i hele meter og kan representere forskjellige forståelser av geografisk presisjon, avhengig av hvordan originaldata er etablert. Generelt for flater vil gjelde at presisjon er et uttrykk for observatørens oppfatning av hvor nøyaktig objektet er geografisk avgrenset/omsluttet på kart i forhold til de faktiske forhold i terrenget. Dette vil også gjelde punktdata i en rekke tilfeller. For punktdata er presisjonen avstanden (radius) mellom midtpunktkoordinatene for det observerte objektet og yttergrensa for det arealet (sirkelflaten) som punktet representerer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktivitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angir type aktivitet som er knyttet til observasjonen/forekomsten. Er bare aktuelt for arter som er mobile og kan ha flere ulike aktiviteter, f.eks. fugl.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>AktivitetKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- stasjonær<br />- muligReproduksjon<br />- næringssøkende<br />- reproduksjon<br />- forflytting<br />- død</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>antallObservasjoner</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Antall observasjoner</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning - artsdata område, for eksempel</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>artsgruppe</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angivelse av  hvilken artsgruppe arten tilhører</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Artsgruppe</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- fugler<br />- karplanter<br />- sopper<br />- insekter<br />- laver<br />- fisker<br />- krepsdyr<br />- moser<br />- pattedyr<br />- øvrigeDyr<br />- alger<br />- edderkoppdyr<br />- amfibierOgReptiler<br />- biller<br />- bløtdyr<br />- koralldyr<br />- mangefotinger<br />- nebbmunner<br />- nettvinger<br />- rettvinger<br />- sekkedyr<br />- sommerfugler<br />- tovinger<br />- vepser<br />- øyenstikkere</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>sted som objektet eksisterer på - artsdata punkt, kan være enkeltobservasjoner eller registreringer</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Point</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>verdikategori</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angivelse av forvaltningskategori</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Verdikategori</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- storVerdi<br />- noeVerdi<br />- sværtStorVerdi<br />- middelsVerdi</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>norskNavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Norsk navn på arten</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>NorskNavn</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>vitenskapeligNavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Vitenskapelig navn</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>VitenskapeligNavn</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="http://skjema.geonorge.no/SOSI/produktspesifikasjon/ArterNasjonalForvaltningsinteresse-2.0/VitenskapeligNavn">http://skjema.geonorge.no/SOSI/produktspesifikasjon/ArterNasjonalForvaltningsinteresse-2.0/VitenskapeligNavn</a></td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>rødlistekategori</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>statuskoder hentet fra Norsk Rødliste for arter og Fremmedartslista</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Rødlistekategori</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Datamangel<br />- Kritisk truet<br />- Livskraftig<br />- Nær truet<br />- Regionalt utdødd<br />- Ikke Vurdert<br />- Sterkt truet<br />- Sårbar</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>artnasjonalId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Ulike kriterier for utvalg</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>maksAntallIndivid</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>utvalgskriterier</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>UtvalgskriteriumKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- ansvarsart – Ansvarsart; Norge har mer enn 25% av arten europeiske bestand<br />- fredet – Fredet art i medhold av naturmangfoldloven<br />- fremmedArt – Fremmed art i Fremmedartslista (Artsdatabanken);
kategoriene Svært høy risiko (SH) og Høy risiko (HI)<br />- prioritert – Prioritert art i medhold av naturmangfoldloven<br />- annenSpesieltHensynskrevende – Annen spesielt hensynskrevende art; andre arter av nasjonal forvaltningsinteresse, utvalgt av Miljødirektoratet<br />- spesielleØkologiskeFormer – Spesiell økologisk form; former eller underarter av arter av nasjonal forvaltningsinteresse som ikke vurderes i rødlisten<br />- nærTruet – Truet art i Norsk rødliste for arter, Norge (Artsdatabanken); kategoriene Kritisk truet (CR), Sterkt truet (EN) og Sårbar (VU)<br />- hensynskrevende<br />- kritiskTruet<br />- sterktTruet<br />- sårbar<br />- datamangel</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Utvalgskriterium</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.ansvarsart</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Ansvarsart; Norge har mer enn 25% av arten europeiske bestand</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.fredet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Fredet art i medhold av naturmangfoldloven</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.fremmedArt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Fremmed art i Fremmedartslista (Artsdatabanken);<br />kategoriene Svært høy risiko (SH) og Høy risiko (HI)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.prioritert</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Prioritert art i medhold av naturmangfoldloven</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.annenSpesieltHensynskrevende</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Annen spesielt hensynskrevende art; andre arter av nasjonal forvaltningsinteresse, utvalgt av Miljødirektoratet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.spesielleØkologiskeFormer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Spesiell økologisk form; former eller underarter av arter av nasjonal forvaltningsinteresse som ikke vurderes i rødlisten</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.nærTruet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Truet art i Norsk rødliste for arter, Norge (Artsdatabanken); kategoriene Kritisk truet (CR), Sterkt truet (EN) og Sårbar (VU)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.hensynskrevende</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.kritiskTruet</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.sterktTruet</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.sårbar</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kriterium.datamangel</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>fraMiljødirektoratet</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sensitivMaskert</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>vitenskapeligNavnId</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>faktaark</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Lenke til faktaark</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Fellesegenskaper_Art

#### Fellesegenskaper_Art (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er fagområde-uavhengige og kan benyttes for naturtype

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unik identifikasjon av et objekt</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Identifikasjon</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjon.lokalId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjon.navnerom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommune</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>nummerering av kommuner i henhold til SSB sin offisielle liste<br /><br />Merknad: Det presiseres at kommune alltid skal ha 4 siffer, dvs. eventuelt med ledende null. Kommune benyttes for kopling mot en rekke andre registre som også benytter 4 siffer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kommunenummer</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="http://register.geonorge.no/sosi-kodelister/kommunenummer.xml">http://register.geonorge.no/sosi-kodelister/kommunenummer.xml</a></td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>datafangstdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

### Kodelister

#### «Enumeration» AktivitetKode

**Definisjon:** angir type aktivitet som er knyttet til observasjonen/forekomsten. Er bare aktuelt for arter som er mobile og kan ha flere ulike aktiviteter, f.eks. fugl.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>stasjonær</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>muligReproduksjon</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>næringssøkende</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>reproduksjon</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>forflytting</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>død</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Artsgruppe

**Definisjon:** angir typen organisme i henhold til en forvaltningsmessig fornuftig inndeling

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>fugler</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>karplanter</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sopper</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>insekter</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>laver</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>fisker</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>krepsdyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>moser</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>pattedyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>øvrigeDyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>alger</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>edderkoppdyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>amfibierOgReptiler</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>biller</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>bløtdyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>koralldyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>mangefotinger</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>nebbmunner</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>nettvinger</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>rettvinger</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sekkedyr</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sommerfugler</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>tovinger</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>vepser</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>øyenstikkere</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Verdikategori

**Definisjon:** kategorisering i ulike grader av forvaltningsinteresse. Inndelingen følger av utvalgskriteriene, slik at hvert utvalgskriterium medfører en bestemt forvaltningskategori.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>storVerdi</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>noeVerdi</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sværtStorVerdi</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>middelsVerdi</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» NorskNavn

**Definisjon:** kodelisten eies og vedlikeholdes av Artsdatabanken og er tilgjengelig som tjeneste "WS_Artsnavnebase" på <a href="http://www2.artsdatabanken.no/artsnavn/Contentpages/Webservices.aspx"><http://www2.artsdatabanken.no/artsnavn/Contentpages/Webservices.aspx></a>

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
  </tbody>
</table>

#### «CodeList» VitenskapeligNavn

**Definisjon:** kodelisten eies og vedlikeholdes av Artsdatabanken og er tilgjengelig som tjeneste "WS_Artsnavnebase" på <a href="http://www2.artsdatabanken.no/artsnavn/Contentpages/Webservices.aspx"><http://www2.artsdatabanken.no/artsnavn/Contentpages/Webservices.aspx></a>

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="http://skjema.geonorge.no/SOSI/produktspesifikasjon/ArterNasjonalForvaltningsinteresse-2.0/VitenskapeligNavn">http://skjema.geonorge.no/SOSI/produktspesifikasjon/ArterNasjonalForvaltningsinteresse-2.0/VitenskapeligNavn</a></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Rødlistekategori

**Definisjon:** statuskoder hentet fra Norsk Rødliste for arter

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Datamangel</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Kritisk truet</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Livskraftig</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Nær truet</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regionalt utdødd</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Ikke Vurdert</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Sterkt truet</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Sårbar</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» UtvalgskriteriumKode

**Definisjon:** Ulike kriterier for utvalg

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ansvarsart</td>
      <td>Ansvarsart; Norge har mer enn 25% av arten europeiske bestand</td>
      <td></td>
    </tr>
    <tr>
      <td>fredet</td>
      <td>Fredet art i medhold av naturmangfoldloven</td>
      <td></td>
    </tr>
    <tr>
      <td>fremmedArt</td>
      <td>Fremmed art i Fremmedartslista (Artsdatabanken);
kategoriene Svært høy risiko (SH) og Høy risiko (HI)</td>
      <td></td>
    </tr>
    <tr>
      <td>prioritert</td>
      <td>Prioritert art i medhold av naturmangfoldloven</td>
      <td></td>
    </tr>
    <tr>
      <td>annenSpesieltHensynskrevende</td>
      <td>Annen spesielt hensynskrevende art; andre arter av nasjonal forvaltningsinteresse, utvalgt av Miljødirektoratet</td>
      <td></td>
    </tr>
    <tr>
      <td>spesielleØkologiskeFormer</td>
      <td>Spesiell økologisk form; former eller underarter av arter av nasjonal forvaltningsinteresse som ikke vurderes i rødlisten</td>
      <td></td>
    </tr>
    <tr>
      <td>nærTruet</td>
      <td>Truet art i Norsk rødliste for arter, Norge (Artsdatabanken); kategoriene Kritisk truet (CR), Sterkt truet (EN) og Sårbar (VU)</td>
      <td></td>
    </tr>
    <tr>
      <td>hensynskrevende</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>kritiskTruet</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sterktTruet</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sårbar</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>datamangel</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Kommunenummer

**Definisjon:** nummerering av kommuner i henhold til Statistisk sentralbyrå sin offisielle liste samt et utvalg av utgåtte numre

Merknad: Det presiseres at kommune alltid skal ha 4 sifre, dvs. eventuelt med ledende null. Kommune benyttes for kopling mot en rekke andre registre som også benytter 4 sifre.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="http://register.geonorge.no/sosi-kodelister/kommunenummer.xml">http://register.geonorge.no/sosi-kodelister/kommunenummer.xml</a></td>
    </tr>
  </tbody>
</table>
