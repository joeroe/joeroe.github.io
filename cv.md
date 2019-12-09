---
title: Cirriculum Vitae
permalink: /cv/
layout: single
---

<address style="text-align: right">
Joe Roe<br/>
Institut for Tværkulturelle og Regionale Studier<br/>
Karen Blixens Plads 8<br/>
2300 København S<br/>
Danmark  
</address>

## Academic employment

`2017–present`
__Department of Cross-Cultural and Regional Studies, University of Copenhagen__
* Research assistant
* Research and teaching post with the [Centre for the Study of Early Agricultural Societies](https://ccrs.ku.dk/research/centres/cseas/) (CSEAS).
* Responsibility for archaeological survey and spatial analysis components of the [Tracking Cultural and Environmental Change](https://tcec.ku.dk/) project and [Shubayqa Archaeological Project](https://shubeika.ccrs.ku.dk/).
* Funded by a research grant from the [C. L. David Foundation](https://www.davidmus.dk/en).


## Education

`2013–present`
__UCL Institute of Archaeology__
* MPhil/PhD in Archaeology
* Thesis: [Modelling prehistoric hunting strategies in Jordan](https://www.ucl.ac.uk/archaeology/people/research/roe). Expected submission 2019.
* Supervisors: [Dr. Louise Martin](https://www.ucl.ac.uk/archaeology/people/staff/lmartin), [Prof. Andrew Bevan](https://www.ucl.ac.uk/archaeology/people/staff/bevan), and [Dr. Andrew Garrard](https://www.ucl.ac.uk/archaeology/people/staff/garrard).
* Supported by [Leverhulme Trust Research Project Grant RPG-2013-223](https://www.leverhulme.ac.uk/funding/grant-schemes/research-project-grants); part of the [Prehistoric Hunting Strategies in Jordan project](https://www.ucl.ac.uk/archaeology/research/directory/prehistoric-hunting-jordan) project.

`2012–2013`
__UCL Institute of Archaeology__
* MA Archaeology (Distinction)
* Taught Masters degree funded by an AHRC Research Preparation Award.
* Dissertation: *Cultural phylogeny of kurgan burial mounds in the west Eurasian steppe* (Supervisor by [Prof. Stephen Shennan](https://www.ucl.ac.uk/archaeology/people/staff/shennan)).
* Subjects studied: GIS in archaeology, spatial analysis, evolution of human cognition, archaeological theory.

`2008–2011`
__University of Durham__
* BA Anthropology and Archaeology (1<sup>st</sup> class hons.)
* Dissertation: *Spatial analysis of intra-site surface collection data from a Cucuteni-Tripolye mega-site*
* Subjects studied: archaeological method and theory, prehistoric archaeology, classical archaeology, landscape archaeology, biomolecular archaeology, cultural anthropology, anthropology of science, biological anthropology, primatology, human behavioural ecology.

`2001–2008`
__Woodkirk High School__


## Grants, awards & scholarships

`2018`
__Det Danske Institut i Damaskus__
* 115,000 DKK grant to support archaeological fieldwork in eastern Jordan (2019). Co-applicant with Tobias Richter.

`2018`
__H. P. Hjerl Hansen Mindefondet for Dansk Palæstinaforskning__
* 50,000 DKK grant to support archaeological fieldwork in eastern Jordan (2019). Co-applicant with Tobias Richter.

`2015`
__UCL Institute of Archaeology__
* Institute of Archaeology Award to support archaeological fieldwork in eastern Jordan.

`2014`
__London Centre for the Ancient Near East__
* Research Students' Conference Grant

`2013`
__Leverhulme Trust__
* PhD Studentship

`2012`
__AHRC__
* Research-preparation Masters Award

## Research interests

* Statistics and computational methods in archaeology
* Quantitive approaches to human palaeo-ecology
* Late Palaeolithic and Neolithic of Southwest Asia, Eastern Europe and the Eurasian steppe
* Archaeological survey and spatial analysis
* Cultural evolution and the application of evolutionary theory to archaeology

## Publications

{% assign papers = site.papers | sort: 'year' | reverse %}
{% for paper in papers %}
* {{ paper.authors_short | default: paper.authors | replace: "Roe, J.", "**Roe, J.**" }} {{ paper.year }}. {{ paper.title }}. *{{ paper.journal }}* {{ paper.volume }}{% if paper.issue %} ({{ paper.issue }}){% endif %}{% if paper.pages %}: {{ paper.pages }}{% endif %}. {% if paper.doi %}[doi:{{ paper.doi }}](https://doi.org/{{ paper.doi }}){% endif %}
{% endfor %}

## Software & datasets

{% assign comps = site.datasets | sort: 'year' | reverse %}
{% for comp in comps %}
* {{ comp.authors_short | default: comp.authors | replace: "Roe, J.", "**Roe, J.**" }} {{ comp.year }}. {{ comp.title }}. *{{ comp.repository }}*. {% if comp.doi %}[doi:{{ comp.doi }}](https://doi.org/{{ comp.doi }}){% endif %}
{% endfor %}

## Field projects

`2019`
__[Shubayqa Archaeological Project](https://shubeika.ccrs.ku.dk/)__
* Co-director (survey)

`2015–2018`
__Shubayqa Archaeological Project__
* Archaeologist/Supervisor
* Survey & excavation

`2018`
__[Ancient Socioecological Systems in Oman (ASOM) project](https://u.osu.edu/asomproject/)__
* Archaeologist
* Survey & excavation

`2015`
__[Kharaneh IV Project](https://kharaneh.wordpress.com/)__
* Archaeologist
* Excavation

`2012–2014`
__[Tripillia Mega-Sites Project](https://www.dur.ac.uk/j.c.chapman/tripillia)__
* Archaeologist/Supervisor
* Survey, excavation & geoarchaeological survey

`2012`
__Mirkovo Project__
* Supervisor
* Survey & excavation

`2012`
__[Gradski Musej Vršac](https://www.muzejvrsac.org.rs/GMVe.htm)__
* Curatorial assistant

`2009`
__Tripillia Mega-Sites Project__
* Trainee
* Survey & excavation

`2007`
__York Archaeological Trust__
* Trainee
* Excavation

## Professional service

`2014–2016`
__*[Papers from the Institute of Archaeology](https://www.pia-journal.co.uk/)*__
* Senior Editor

`2014–2016`
__UCL Institute of Archaeology__
* Postgraduate Student Representative

`2013–2014`
__*Papers from the Institute of Archaeology*__
* Editorial Assistant

## Conference, seminar & workshop participation

{% assign presentations = site.talks | concat: site.posters | sort: 'year' | reverse %}
{% for presentation in presentations %}
* {{ presentation.authors_short | default: presentation.authors | replace: "Roe, J.", "**Roe, J.**" }} {{ presentation.year }}. *{{ presentation.title }}*{% if presentation.preview %} (poster){% endif %}. Presented at {{ presentation.conference }}.
{% endfor %}

## Conference organisation

`2019`
__[Computer Applications & Quantitative Methods in Archaeology (CAA) 2019](https://2019.caaconference.org/), Kraków__
* Session organiser (with Francesco Carrer) 
* S06, *Recent advances in spatial statistics for archaeology*

`2014`
__[Postgraduate Zooarchaeology Forum (PZAF) 2014](https://pzaf2014.wordpress.com/), London__
* Conference organiser

## Teaching & public engagement

`2015–2016`
__UCL Institute of Archaeology__
* Postgraduate Teaching Assistant
* ARCL2028 Research & Presentation Skills

`2014–2016`
__[The Brilliant Club](https://www.thebrilliantclub.org/)__
* Tutor
* As a Brilliant Club tutor, I developed an intensive tutorial course based on my PhD research and delivered it to groups of high performing pupils in low participation schools across London.

`2015`
__Petrie Museum of Egyptian Archaeology__
* Student Volunteer, 'Maths and Archaeology' workshop
* Outreach event for high school students organised by Dr. Alice Stevenson (Petrie Museum) and Dr. Luciano Rila (UCL Mathematics) and supported by the London Mathematical Society.

## Professional memberships

`2014–present`
__[Council for British Research in the Levant](http://cbrl.ac.uk/) (CBRL)__

`2014–present`
__[Computer Applications and Quantitative Methods in Archaeology](https://caa-international.org/) (CAA)__

## Other employment & volunteering

`2010–present`
__English Wikipedia__
* Editor, community-appointed administrator and elected member of the Arbitration Committee (2019–2020)

`2018`
__Kirklees Citizens Advice Bureau__
* Gateway Advisor

`2012`
__TPP SystmOne__
* Software Engineer
* Data migration and front-end programming for a large clinical systems developer.
