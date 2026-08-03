---
title: "Archaeological Information Systems: A Comparison of Field Recording Software (updated 2026)"
description: "A comparison of archaeological information systems (AIS) including ARCHES, ARK, Field, FAIMS, Ishtar, Kiosk, OpenAtlas, ArcheoBase, Diggit, Intrasis, and MuseumsGIS, with metadata, feature comparisons, and assessments from a research archaeologist's perspective."
classes: "narrow" # override site config
toc: true
toc_sticky: true
---

This page provides an up-to-date comparison of available **archaeological information systems**,
including ARCHES, ARK, Field, FAIMS, Ishtar, Kiosk, OpenAtlas, ArcheoBase, Diggit, Intrasis, and MuseumsGIS.

See [updates](#updates) below for information on changes since the page was first published.

## What is an 'archaeological information system'?

I define an 'archaeological information system' (AIS) as software specifically developed for the recording, management and publication of field archaeological data, including both excavations and surveys.
It is not a widely used term (though I am not the first to use it), but I think usefully captures a particular type of system which is to archaeology what a geographical information system (GIS) is to geospatial applications.

It is worth noting that the most commonly used archaeological information system *is* a geographic information system (see [honourable mentions](#honourable-mentions) below).
The development of specific software to extend or replace GIS for in archaeological fieldwork is a relatively new phenomenon.
In some contexts (e.g. rescue archaeology in particular countries), one or another AISes have become the norm;
but in globally the field still seems to prefer GIS- and/or paper-based recording systems.
This makes AIS a rather interesting, experimental niche within archaeological research software engineering.

## Summary of available archaeological information systems

| Software                                         | Developer                         | Open source | Self-hostable | Price                                    | Notable users                             |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [ARCHES](https://www.archesproject.org/)         | 🇺🇸 Getty Conservation Institute | ✅          | ✅            | Free                                     | UK Historic Environment Registers         |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [ArcheoBase](https://archeobase.org/)            | 🇨🇭 AnalyticBase Sàrl            | ❌          | ❌            | 23 CHF per user per month                | Swiss cantonal archaeological services    |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [ARK](https://ark.lparchaeology.com/)            | 🇬🇧 L-P Archaeology              | ✅          | ✅            | Free                                     |                                           |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [Diggit](https://www.diggitarchaeology.com/)[^1] | 🇬🇧 Diggit Archaeology           | ❌          | ❌            | 1 GBP per context                        |                                           |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [Field](https://github.com/dainst/idai-field)    | 🇩🇪 DAI                          | ✅          | ✅            | Free                                     | German Archaeological Institute branches  |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [FAIMS](https://faims.edu.au/)                   | 🇦🇺 Macquarie University / CSIRO | ✅          | ✅            | Free                                     |                                           |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [Intrasis](https://www.intrasis.com/)            | 🇸🇪 Arkeologerna                 | ❌          | ✅            | 21,000 SEK                               | Swedish & Danish museums                  |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [Ishtar](https://ishtar-archeo.net/en/)          | 🇫🇷 Iggdrasil                    | ✅          | ✅            | Free                                     |                                           |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [Kiosk](https://sites.brown.edu/kiosk/)          | 🇺🇸 Brown University             | ✅          | ✅            | Free                                     |                                           |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [MuseumsGIS](https://www.museumsgis.dk/)[^2]     | 🇩🇰 Arkæologisk IT               | ?           | ?             | c. 37,000 DKK per year                   | Danish museums                            |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|
| [OpenAtlas](https://openatlas.eu/)               | 🇦🇹 Austrian Academy of Sciences | ✅          | ✅            | Free                                     |                                           |
|--------------------------------------------------|-----------------------------------|-------------|---------------|------------------------------------------|-------------------------------------------|

## How to choose an archaeological information system?

In the tables here I have compiled basic metadata and feature information on archaeological information systems that are actively maintained.
Metadata includes the licensing and price model, developer, and notable users.
The feature comparison includes major points of differentiation between the different software; 
features that all systems offer, like data input or file export, are not included.

I have paid particular attention to whether the system is free and open source or commercial, and in which case how much.
This is because I usually advocate for the use of free and open source software in academic contexts.
Since archaeological information systems are used primarily for data management, rather than an analysis, I would not say that a free and open source software is *essential* in this case.
However, is still offers distinct advantages in terms of interoperability and maintainability (allowing a wider community to share the development burden) and, in an educational context, avoiding locking students into proprietary walled gardens early in their career.
That said, the current reality is that some of the best systems are commercial.

My assessments below are written from the perspective of a research archaeologist based at a university, on the basis of the information I could find and demo versions available.
I have tried to keep up to date with this field over the years out of a theoretical interest.
If I were to use any of the systems myself, it would be in a seasonal research-led field projects and in an educational context, where I want to expose (Danish) students in the modern recording systems they are likely to encounter in their future careers.
I am not in a position to evaluate their usefulness to larger institutions or in commercial archaeology contexts, nor to trial each system in the field.
Some systems I have not been able to try at all; where this is the case, it is noted below.

## Feature comparison

| Feature           | ARCHES | ArcheoBase | ARK | Diggit | Field | FAIMS | Intrasis | Ishtar | Kiosk | MuseumsGIS | OpenAtlas |
|-------------------|--------|------------|-----|--------|-------|-------|----------|--------|-------|------------|-----------|
| Mobile app        | ❌     | ✅         | ❌  | ✅     | ❌    | ✅    | ✅       | ❌     | ✅    | ✅         | ❌        |
| Offline recording | ❓     | ❓         | ❌  | ✅     | ✅    | ✅    | ❓       | ❌     | ✅    | ❓         | ❌        |
| Harris matrix     | ❓     | ✅         | ✅  | ❓     | ✅    | ❌    | ❓       | ✅     | ✅    | ❓         | ❓        |
| Mapping           | ✅     | ❓         | ✅  | ❌     | ✅    | ✅    | ✅       | ✅     | ❓    | ✅         | ✅        |
| GIS integration   | ✅     | ❓         | ✅  | ✅     | ✅    | ✅    | ✅       | ✅     | ❓    | ✅         | ✅        |
| Public portal     | ✅     | ✅         | ✅  | ❓     | ❓    | ❌    | ❓       | ✅     | ❓    | ✅         | ✅        |

Mobile app
: Dedicated application for iOS or Android devices

Offline recording
: Ability to record data without internet connectivity

Harris matrix
: Built-in tool for generating stratigraphic relationship diagrams

Mapping
: In-app capability to input spatial data (points, lines, polygons)

GIS integration
: Ability to export to or integrate with external GIS software (QGIS, ArcGIS, etc.)

Public portal
: Web interface for public access to project data

## Honourable mentions

Apart from dedicated software, archaeologists routinely make their own digital recording systems with off-the-shelf database (e.g. FileMaker, Microsoft Access) or geographic information system (GIS; e.g. QGIS, ArcGIS) software.
In recent years, the availability of mobile GIS apps such as QField and ArcGIS Field Maps have made the latter particularly popular solutions.

These DIY approaches are popular for good reasons.
They offer flexibility to adapt to specific project needs, lower cost (especially with open source tools), and no vendor lock-in.
They also allow archaeologists to leverage existing skills and workflows rather than learning new systems.
For small projects or research-led fieldwork, a custom solution can be more practical than adopting a full archaeological information system.
For example, I've been using a [QGIS-based DIY field recording stack](/posters/2019/caa2019_qcontinuum.html) for research-led field surveys for nearly a decade and it works well.
It's customised to my specific needs, is free and open source, and integrates seamlessly with my analysis workflows.

However, there are trade-offs.
DIY systems require technical expertise to set up and maintain, and there's no dedicated support when things go wrong.
Each project essentially reinvents the wheel, making it harder to share data and workflows between projects or institutions.
Still, I'd guess that the combined use of these DIY systems is significantly greater than any software developed specifically for archaeology.
But as my focus here is on explicit archaeological information systems, I won't consider them further.

## Free and open source archaeological information systems

### ARCHES

[ARCHES](https://www.archesproject.org/) is a web-based, self-hosted heritage data management platform developed by the [Getty Conservation Institute](https://www.getty.edu/conservation) and [World Monuments Fund](https://www.wmf.org).
It was originally designed for inventories of immovable cultural heritage and has been widely adopted by Historic Environment Records in the United Kingdom, which are served by a dedicated version called [Arches for HERs](https://www.archesproject.org/arches-for-hers/).
It has also been adopted by projects including Endangered Archaeology in the Middle East and North Africa (EAMENA) at Oxford[^3] and the Greater London Historic Environment Record.[^4]
The system includes GIS functionality.
It requires technical expertise to deploy and maintain.

ARCHES is a sophisticated and mature system with significant institutional backing from major organisations.
However, it is primarily tailored for heritage management and inventory purposes, and its utility for active field recording remains unclear.
The system is also notably complex to deploy and maintain, requiring substantial technical expertise that may be prohibitive even for experienced system administrators without dedicated IT support.

### ARK

[ARK](https://ark.lparchaeology.com/) (Archaeological Recording Kit) is a web-based, self-hosted system developed by [L-P Archaeology](https://www.lparchaeology.com/).
It provides an interface for data entry, editing, mapping, and sharing of archaeological project data, and supports web services and data export.
It has been used on excavations including the Villa Magna project in Italy[^5] and Portus.[^6]

ARK was an early pioneer of web-based archaeological recording and represented an important step forward in the digitisation of field documentation.
However, the system has not been actively maintained or updated since 2014, and its underlying technology stack has become dated.
The web-based architecture limits its practical utility in remote field locations where reliable internet connectivity cannot be assumed, and the older codebase presents significant barriers to long-term maintainability and future development.

### Field

[Field](https://github.com/dainst/idai-field) (formerly iDAI.field) is a desktop application (with optional sync server) developed by the [German Archaeological Institute](https://www.dainst.org) (DAI) and the [GBV Common Library Network](https://en.gbv.de/).
It allows archaeologists to record, share, and store excavation data and images, customise data models, map records, manage types and inventories, and synchronise data.
The system comprises a desktop application (Angular/Electron), a mobile app (React Native, in early development), and an optional sync server.

Field represents a very promising and full-featured approach to archaeological data management, backed by a sizeable research software engineering team and the international presence of the German Archaeological Institute.
The involvement of DAI branches across multiple countries provides both development capacity and a built-in user base that lends the project considerable institutional weight and long-term viability.
It does not yet have a mobile application, which is increasingly seen as essential for modern in-field recording workflows.
However, a mobile app is actively under development in React Native.

### FAIMS

[FAIMS](https://faims.edu.au/) (Field Acquired Information Management Systems) is an open source platform for offline field data collection, originally developed for archaeology but now used across multiple disciplines including geoscience and humanities.
The project has an 11-year development history since 2012, with a major rebuild as FAIMS 3.0 released in 2022.
It is cross-platform (Android, iOS, and desktop) and offers a self-service notebook designer for customization without coding.
Features include offline data capture, mobile GIS, annotations, certainty sliders, multimedia support, and version control.
In 2023, the software was rebranded as Fieldmark™ with a commercial hosting option, though the open source version remains freely available.

FAIMS has been used in over 40 projects and demonstrates a long-term commitment to offline-first field recording.
However, based on experience with earlier versions, the system can be difficult to set up and the data model prioritises flexibility over out-of-the-box utility for archaeological workflows.
The cross-disciplinary nature of the platform is both a strength (allowing adaptation to diverse research needs) and a weakness (requiring more customization than archaeology-specific systems).
The institutional backing from Macquarie University, CSIRO, and the Australian Research Data Commons provides stability, and the complete rebuild in FAIMS 3.0 may address earlier usability concerns.

### Ishtar

[Ishtar](https://ishtar-archeo.net/en/) is a web-based, self-hosted system developed by the French company [Iggdrasil](https://www.iggdrasil.net/).
It manages data from excavation through to museum storage, including context records, finds, administrative files, warehouses, and conservatory treatments.
The system has a modular architecture (cartography, underwater archaeology, public portal, etc.) with customisable forms, automatic inventory generation, and multiple user permission levels.
First released in 2017, version 4 was released in 2024.

I have not yet had the opportunity to trial this system in practice. Further assessment will be provided once hands-on evaluation has been conducted.

### Kiosk

[Kiosk](https://sites.brown.edu/kiosk/) is an iPad-based, self-hosted digital field recording platform developed and maintained at Brown University.
It is designed to work offline in remote locations, with data synchronisation possible without internet access.
It supports excavation and pedestrian survey recording, Harris matrices, ceramic analysis, custom numbering systems, and legacy data integration.
It is used by institutions including NYU, University of Chicago, and Leiden University.

Kiosk's restriction to the iOS ecosystem represents a significant limitation, particularly for a free and open source application.
This platform dependency precludes trialling the system on non-Apple devices and may exclude many potential users whose institutions have standardised on Android or mixed-device environments.
For a FOSS project, such vendor lock-in is especially unfortunate and runs counter to the principles of accessibility and platform independence that typically characterise open source software.

### OpenAtlas

[OpenAtlas](https://openatlas.eu/) is a web-based, self-hosted database application developed by the [Austrian Centre for Digital Humanities](https://www.oeaw.ac.at/acdh) (ACDH), an institute of the [Austrian Academy of Sciences](https://www.oeaw.ac.at/), for managing research data across the humanities.
It provides customisable forms for recording complex relationships.
Features include an interactive Leaflet-based map with PostGIS spatial data, Linked Open Data reference systems, and data integrity checks.
It is used by the Österreichisches Archäologisches Institut and other partner projects.[^7]

OpenAtlas is a mature and well-established system with strong institutional backing from the Austrian Archaeological Institute.
Like ARCHES, however, it appears to be oriented more towards heritage management, inventory control, and long-term data curation than towards the practical demands of active field recording.
Its sophisticated data model and emphasis on complex relational structures may be better suited to post-excavation analysis and museum collections management than to the rapid, context-by-context documentation required during excavation.

## Commercial archaeological information systems

### ArcheoBase

[ArcheoBase](https://archeobase.org/) is a cloud-based SaaS platform developed by the Swiss company [AnalyticBase Sàrl](https://archeobase.org/).
It covers the full chain of archaeological information processing through modular sub-applications: Archeo Entry (data input), Archeo Analysis, Archeo Publication, Archeo View (public dissemination), Archeo Forum (community), and Archeo Archive.
Available in multiple European languages, it is priced at 23 CHF per user per month and offers a mobile app for field recording.

ArcheoBase presents a very comprehensive and well-designed system with an impressive range of features covering the full spectrum of archaeological information management.
The modular architecture and multilingual support demonstrate careful attention to user needs.
The pricing model does not work well in a research context, where fieldwork is seasonal and typically involves large numbers of temporary staff.
The developers have indicated they are introducing a new pricing plan specifically for universities, which may address this concern if implemented at a level accessible to academic institutions.

### Diggit

[Diggit](https://www.diggitarchaeology.com/) is a cloud-based SaaS recording system developed by [Diggit Archaeology](https://www.diggitarchaeology.com/) (UK).
It consists of a mobile app (diggitmobile) for on-site recording and a web interface (diggitweb) for exploration, analysis, and export.
The interface includes over 240 archaeology-specific icons and charges per context recorded (1 GBP).
It is currently available only in the UK, Ireland, and Hong Kong.

Diggit employs an interesting and unconventional pricing model based on the number of contexts recorded rather than the number of users.
While this could be advantageous for small projects with limited recording needs, it makes costs difficult to predict and budget for larger excavations where the volume of contexts is uncertain.
The system is currently available only in the United Kingdom, Ireland, and Hong Kong, making it inaccessible for evaluation in other regional contexts.
As it is not available in Denmark, I was unable to conduct a trial assessment of its capabilities and workflow.

### Intrasis

[Intrasis](https://www.intrasis.com/) is a desktop application (with optional cloud sync) originally designed by [Arkeologerna](https://arkeologerna.com/en/) (The Archaeologists) at the Swedish National Historical Museums agency.
It combines a database with geographical information for documenting, visualising, and analysing excavation data.
While proprietary, it is self-hostable and offers both desktop and mobile apps.
According to their website, "it additionally requires an ArcGIS license with minimum licensing to ArcGIS engine runtime (included in ArcGIS desktop)."[^8]
It is used by Swedish and Danish museums.
The latest version (4.2) runs on PostgreSQL and includes 3D visualisation capabilities.

Intrasis has a rather complex pricing model with various licence types and add-ons.
A single-use licence costs 21,000 SEK as a one-time fee, while educational packages are available at 10,000 SEK per year.
For full details on licensing options, see the [Intrasis pricing page](https://www.intrasis.com/faq/lisencing-and-prices/).

Intrasis is one of the longest-established archaeological information systems and has achieved significant adoption in commercial archaeology in Sweden and, to a lesser extent, within the Danish museum system.
However, the system's hard dependency on proprietary ESRI ArcGIS software represents a fundamental barrier to adoption for many users.
At a time when open source GIS solutions such as QGIS have become mature, widely-used, and well-supported within the archaeological community, requiring users to maintain expensive proprietary GIS licenses alongside Intrasis is increasingly difficult to justify.

### MuseumsGIS

[MuseumsGIS](https://www.museumsgis.dk/) is a web-based system with mobile app developed by [Arkæologisk IT](https://moesgaardmuseum.dk/om-moesgaard/forskning-og-viden/arkaeologisk-it) at Moesgaard Museum, Denmark.
It is currently only available to Danish museums.
It is built on free and open source software but requires a licence to use, costing approximately 37,000 DKK per year.
It comprises a project presentation website (dynamically pulling excavation data including 3D models, historical maps, and geophysics), a mobile field registration app, and QGIS plugins including the FeltTegn tool for converting GPS data to archaeological features.
Data is stored on a central database server with full version history at the object level, and is immediately available to both mobile devices and QGIS.

MuseumsGIS is relatively new with a very impressive feature set that addresses many of the practical requirements of modern archaeological recording:
integration of 3D models, geophysical data, and real-time synchronisation between field devices and QGIS.
It is currently tightly tailored to the Danish museum sector in its design and pricing;
but the fact that it is built on an open source technology stack means that, in principle, the system could be forked and adapted by other institutions or communities.

## Updates

I will keep this page updated as often as possible.
Please feel free to contact me with updates, corrections, or suggested additions.

* 2026-08-03: first version

## References

[^1]: Diggit is only available in the United Kingdom, Ireland, and Hong Kong.  
[^2]: MuseumsGIS is only available in Denmark.
[^3]: [EAMENA database](https://eamena.org/database)
[^4]: [GLHER](https://glher.historicengland.org.uk/)
[^5]: [Villa Magna](https://ark.lparchaeology.com/portfolio/villa-magna/)
[^6]: [Portus](https://ark.lparchaeology.com/portfolio/portus/)
[^7]: [THANADOS](https://thanados.net)
[^8]: [Intrasis - What is Intrasis?](https://www.intrasis.com/what-is-intrasis/)

