# Lovdata Public Datasets

This repository mirrors the freely available Lovdata public law datasets published under the NLOD 2.0 license. Each archive contains HTML/XML representations of Norwegian statutes and central regulations.

## Bundles

- `gjeldende-lover.tar.bz2` – Current consolidated statutes with amendments.
- `gjeldende-sentrale-forskrifter.tar.bz2` – Current nationwide regulations with amendments.
- `lovtidend-avd1-2025.tar.bz2` – 2025 Norsk Lovtidend Section I releases (laws and central regulations).
- `lovtidend-avd1-2001-2024.tar.bz2` – Historical Norsk Lovtidend Section I releases from 2001 through 2024.

For details on the dataset structure and terms, see https://api.lovdata.no/.

## Curated subsets

- `real-estate/nl/` – 25 high-value statutes within the Lovdata “gjeldende lover” export that govern Norwegian real-estate transactions, tenure, registration, and neighbor relations. Files retain the original Lovdata HTML/XML structure for downstream processing. Highlights include:
  - Transaction & tenure: `nl-19920703-093.xml` (Avhendingslova), `nl-19990326-017.xml` (Husleieloven), `nl-19961220-106.xml` (Tomtefestelova), `nl-20170616-065.xml` (Eierseksjonsloven), `nl-20030606-038.xml`/`039.xml` (Bustadbyggjelagslova/Burettslagslova).
  - Registration & mapping: `nl-19350607-002.xml` (Tinglysingsloven), `nl-20050617-101.xml` (Matrikkellova), `nl-20100903-056.xml` (Geodataloven), `nl-20070629-073.xml` (Eiendomsmeglingsloven).
  - Land-use powers & neighbor law: `nl-19170601-001.xml` (Skjønnsprosessloven), `nl-19591023-003.xml` (Oreigningslova), `nl-19610505-000.xml`/`nl-19610616-015.xml` (Grannegjerdelova/Grannelova), `nl-19840406-017.xml` (Ekspropriasjonserstatningslova), `nl-20250620-093.xml` (plan- og bygningsloven/matrikkellova amendments).

Use this folder when you need a narrow, property-focused law set for search/RAG pipelines without unpacking the entire Lovdata drops. Each filename matches the official Lovdata identifier so updates can be automated with the same filters (e.g., `legalArea` contains “Fast eiendoms rettsforhold”).
