# Chci být Pražák nebo "dojížďák"
projekt v **Digitální Akademii DATA (Czechitas)**

## O Projektu
**Cíl projektu:** Porovnání **cen nemovitostí** v Praze a Středočeském kraji a návrh interaktivního nástroje, který pomůže s výběrem lokality ke koupi nemovitosti. Zkoumaly jsme **dojezdovou vzdálenost a dobu** z obcí Středočeského kraje a nemovitostí v Praze (zde jen hromadná doprava).

## Zdrojové kódy
Naleznete tu dva hlavní soubory, ve kterých najdete kódy pro získávání tras

### 1. Cesta autem
- **soubor**: keboola_transformace.ipynb
- **popis:** Kód, který se používal v rámci Flow v Keboole pro automatizované volání REST API Mapy.cz, včetně současné dopravní situace.

### 2. Hromadná doprava
- **soubor**: jizdni_rady_v5.ipynb
- **popis**: Kód pro získávání informací o trase hromadnou dopravou, včetně transformace a logiky najít nejrychlejší trasu, trasu s nejméně přestupy (ale omezení na chůzi, protože někdy byly úseky chůze na začátku a konci trasy velmi dlouhé) a případně vlakových spojů.
- Jednotlivé varianty dopravy vyžadují drobné odlišnosti, i když základní struktura kódu je stejná. Takže se nedobje, nejedná se duplicity.
- **Zdroj dat**: OTP2 (GraphQL API) - vychází z OSM souboru Čerské Republiky a aktuálních jízdních řádů ROPID ve formátu GTFS


