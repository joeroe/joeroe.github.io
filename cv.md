---
title: Curriculum Vitae
permalink: /cv/
layout: single
toc: true
toc_label: "Contents"
toc_sticky: true
classes: ""
---

<address>
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
* Thesis: [Modelling prehistoric hunting strategies in Jordan](https://www.ucl.ac.uk/archaeology/people/research/roe). Expected submission 2020.
* Supervisors: [Dr. Louise Martin](https://www.ucl.ac.uk/archaeology/people/louise-martin-reader-zooarchaeology), [Prof. Andrew Bevan](https://www.ucl.ac.uk/archaeology/people/andrew-bevan-professor-spatial-and-comparative-archaeology), and [Dr. Andrew Garrard](https://www.ucl.ac.uk/archaeology/people/andrew-garrard-associate-professor-early-prehistory).
* Supported by Leverhulme Trust Research Project Grant RPG-2013-223; part of the [Prehistoric Hunting Strategies in Jordan project](https://www.ucl.ac.uk/archaeology/research/directory/prehistoric-hunting-strategies-jordan) project.

`2012–2013`
__UCL Institute of Archaeology__
* MA Archaeology (Distinction)
* Taught Masters degree funded by an AHRC Research Preparation Award.
* Dissertation: *Cultural phylogeny of kurgan burial mounds in the west Eurasian steppe* (supervised by [Prof. Stephen Shennan](https://www.ucl.ac.uk/archaeology/people/stephen-shennan-professor-theoretical-archaeology))
* Subjects studied: GIS in archaeology, spatial analysis, evolution of human cognition, archaeological theory.

`2008–2011`
__University of Durham__
* BA Anthropology and Archaeology (1<sup>st</sup> class hons.)
* Dissertation: *Spatial analysis of intra-site surface collection data from a Cucuteni-Tripolye mega-site* (supervised by [Prof. John Chapman](https://www.dur.ac.uk/archaeology/staff/?id=150))
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

* Computational archaeology and archaeostatistics
* Human palaeoecology
* Palaeolithic and Neolithic of Southwest Asia, Eastern Europe and the Eurasian steppe
* Digital recording and informatics in archaeological survey
* Cultural evolution and evolutionary theory in archaeology

## Publications

{% assign papers = site.papers | sort: 'year' | reverse %}
{% for paper in papers %}
* {{ paper.authors_short | default: paper.authors | replace: "Roe, J.", "**Roe, J.**" }} {% if paper.in_press %}in press{% elsif paper.submitted %}in prep{% else %}{{ paper.year }}{% endif %}. {{ paper.title }}. {% if paper.book %}In {{ paper.editors_short }} (eds.), *{{ paper.book }}*{% if paper.pages %}, pp. {{ paper.pages }}. {% endif %}{% elsif paper.submitted %}Manuscript submitted for publication.{% else %}*{{ paper.journal }}* {{ paper.volume }}{% if paper.issue %} ({{ paper.issue }}){% endif %}{% if paper.pages %}: {{ paper.pages }}. {% endif %}{% endif %}{% if paper.publisher %}{{ paper.publisher }}. {% endif %}{% if paper.doi %}[doi:{{ paper.doi }}](https://doi.org/{{ paper.doi }}){% endif %}
{% endfor %}

## Software & datasets

{% assign comps = site.datasets | concat: site.code | sort: 'year' | reverse %}
{% for comp in comps %}
* {{ comp.authors_short | default: comp.authors | replace: "Roe, J.", "**Roe, J.**" }} {{ comp.year }}. {{ comp.title }}. {% if comp.repository %}*{{ comp.repository }}*.{% endif %} {% if comp.doi %}[doi:{{ comp.doi }}](https://doi.org/{{ comp.doi }}).{% endif %} {% if comp.website %}<{{ comp.website }}>.{% endif %}
{% endfor %}

## Field projects

`2019`
__[Shubayqa Archaeological Project](https://shubeika.ccrs.ku.dk/)__
* Co-director (survey)

`2015–2018`
__Shubayqa Archaeological Project__
* Field archaeologist & supervisor

`2018`
__[Ancient Socioecological Systems in Oman (ASOM) project](https://u.osu.edu/asomproject/)__
* Field archaeologist

`2015`
__[Kharaneh IV Project](https://kharaneh.wordpress.com/)__
* Field archaeologist

`2012–2014`
__[Tripillia Mega-Sites Project](https://www.dur.ac.uk/j.c.chapman/tripillia)__
* Field archaeologist & supervisor

`2012`
__Mirkovo Project__
* Supervisor

`2009`
__Tripillia Mega-Sites Project__
* Trainee

`2007`
__York Archaeological Trust__
* Trainee

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

## Conference presentations

{% assign presentations = site.talks | concat: site.posters | sort: 'year' | reverse %}
{% for presentation in presentations %}
* {{ presentation.authors_short | default: presentation.authors | replace: "Roe, J.", "**Roe, J.**" }} {{ presentation.year }}. *{{ presentation.title }}*{% if presentation.preview %} (poster){% endif %}. Presented at {{ presentation.conference }}.
{% endfor %}

## Conference organisation

`2019`
__[Computer Applications & Quantitative Methods in Archaeology (CAA) 2019](https://2019.caaconference.org/), Kraków__
* Session organiser (with Francesco Carrer): S06, *Recent advances in spatial statistics for archaeology*

`2014`
__[Postgraduate Zooarchaeology Forum (PZAF) 2014](https://pzaf2014.wordpress.com/), London__
* Conference organiser

## Workshop & seminar participation

`2019`
__Computer Applications & Quantitative Methods in Archaeology (CAA) 2019, Kraków__
* Roundtable discussant: S03, *Scientific Scripting Languages in Archaeology: Limits and Opportunities of Open Research*

`2018`
__Christian-Albrecht University of Kiel__
* International Summer School, "Connecting the Dots"
  * Development of the R package [moin: Modeling Interaction in Landscape Archaeology](https://github.com/ISAAKiel/SummerSchool_moin)

`2017`
__University of Copenhagen__
* Shubayqa Project Workshop

`2016`
__University of Nottingham__
* Workshop, "Near East Climate"
  * Invited to international workshop organised by Prof. Matthew Jones, basis for publication of [Jones et al. 2019](/papers/2019/climate_change_in_southwest_asia.html).

## Teaching & public engagement

`2018–present`
__Department of Cross-Cultural and Regional Studies, University of Copenhagen__
* Lecturer on courses:
  * BA: "Practical Archaeology 1" (*Arkæologisk praksis 1*, [HNAB0100FU](https://kurser.ku.dk/course/hnab0100fu/)), "Practical Archaeology 2" (*Arkæologisk praksis 2*, [HNAB0102EU](https://kurser.ku.dk/course/hnab0102eu/)), "Science and Theory of Science" (*Videnskabsteori*, [HTOR0102FU](https://kurser.ku.dk/course/htor0102fu/))
  * KA: "Theory and Method in Near Eastern Archaeology" ([HNAK0101EU](https://kurser.ku.dk/course/hnak0101eu/)), "Environments and landscapes in the archaeological record of southwest Asia" ([HNAB0102FU](https://kurser.ku.dk/course/hnab0102fu/)), "Neolithic to Early Urban Periods in the Near East" ([HNAK0102EU](https://kurser.ku.dk/course/hnak0102eu/)), "Project-based course" ([HNAK0100FU](https://kurser.ku.dk/course/hnak0100fu/))
* Organiser of a two-day workshop on mobile GIS for linguistic field research

`2020`
__University of Pisa__
* Instructor: [Winter School: R for Archaeologists](http://www.mappaproject.org/r4rchaeologists/)

`2015–2016`
__UCL Institute of Archaeology__
* Postgraduate Teaching Assistant: ARCL2028 Research & Presentation Skills

`2014–2016`
__[The Brilliant Club](https://www.thebrilliantclub.org/)__
* Tutor
* Developed an intensive tutorial course based on my PhD research and delivered it to groups of high performing pupils in low participation schools across London.

`2015`
__Petrie Museum of Egyptian Archaeology__
* Student Volunteer, *Maths and Archaeology* workshop
* Outreach event for high school students organised by Dr. Alice Stevenson (Petrie Museum) and Dr. Luciano Rila (UCL Mathematics) and supported by the London Mathematical Society.

## Professional memberships

`2020–present`
__[Society of Research Software Engineering](https://society-rse.org/) (RSE)__

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
__[Gradski Musej Vršac](https://www.muzejvrsac.org.rs/GMVe.htm)__
* Curatorial assistant

`2012`
__TPP SystmOne__
* Software Engineer
* Data migration and front-end programming for a large clinical systems developer.
