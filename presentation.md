class: middle, center

# Data wrangling

### Lessons learned during SAFRED data processing

Safeguarding Biodiversity Data for the Future<br>
27 February 2018

Stijn Van Hoey

[<i class="fa fa-twitter"></i> @SVanHoey](https://twitter.com/svanhoey) [<i class="fa fa-github"></i> stijnvanhoey](https://github.com/inbo)

---
class: middle, center, section_background

# What's up with my data?

---
class: middle

> "... farmland ponds distributed over almost the entire **Belgian territory**."

.center[![:scale 95%](./static/images/coordinates_1.png)]

---
class: middle

> "... farmland ponds distributed over almost the entire **Belgian territory**."

.center[![:scale 95%](./static/images/coordinates_2.png)]

---
class: middle

> color annotations ...

.center[![:scale 95%](./static/images/color_usage_1.png)]

---
class: middle

> color annotations ...

.center[![:scale 95%](./static/images/color_usage_2.png)]

---
class: middle

> * measurementUnits are constraints
> * measurementValues don't follow constraints

id | measurementType | measurementValue | measurementUnit
--- | --- | --- | ---
HnPloEx_2003 | URBAN_400 | 1.193662073 | 0/1
WVIepIn_2003 | FOREST_100 | 1.193821228 | 0/1
VBHalEx_2003 | FOREST_1600 | 1.206983342 | 0/1
VBDieNa_2003 | FOREST_200 | 1.222572569 | 1/2/3/4
LiVoeIn_2003 | FOREST_400 | 1.247465892 | 1/2/3/4
WVKnoEx_2003 | URBAN_200 | 1.255517642 | 1/2/3/4

---
class: middle

> * lowercase/uppercase issues with identifiers
> * a value `782?` for conductivity
> * trailing white spaces for scientific names
> * encoding issue with units
> * remarks column wrongly included when pivoting
> * ...

---
class: middle, center

![:scale 75%](./static/images/keep-calm-and-clean-up-the-mess.png)

---
class: middle, center, section_background

# From `any format` to a standard

---
class: middle, center

## Initial MANSCAPE workflow

![:scale 85%](./static/images/workflow_1.png)

---
class: middle, center

## Initial MANSCAPE workflow

![:scale 85%](./static/images/workflow_2.png)

---
class: middle, center, section_background

# A reproducible workflow

---
class: middle, center

![:scale 85%](./static/images/workflow_5.png)

---
class: middle, center, subsection_background

#  Literate programming

---
class: middle, center

## Python

![:scale 100%](./static/images/literate_programming_python.png)

---
class: middle, center

## R

![:scale 100%](./static/images/literate_programming_R.png)

---
class: middle, center

## Executable documentation

> ... in literate programming the emphasis is reversed. Instead of writing code containing documentation, the literate programmer writes `documentation containing code`

--

.footnote[Jupyter notebook supports > 40 programming  languages, Rmarkdown rocks for R users!]

---
class: middle, center, subsection_background

#  Version control

---
class: middle, center

![:scale 100%](./static/images/gists_revisions.png)

---
class: middle, center

![:scale 100%](./static/images/version_control_1.png)

---
class: middle, center

.center[![:scale 100%](./static/images/version_control_2.png)]

---
class: middle, center

## A reproducible workflow

![:scale 85%](./static/images/workflow_3.png)

---
class: middle, center

## A reproducible workflow

![:scale 85%](./static/images/workflow_4.png)

.footnote[*Python `Pandas` or R `dplyr` provide most of the functionalities]

---
class: middle, center, section_background

#  We all make mistakes! 

---
class: middle, center

![:scale 100%](./static/images/workflow_6.png)

---
class: middle, center

## How to check  if a dataset fits the data quality `requirements`?

---
class: middle, center

## Let's `document` those

---
class: middle, center

![:scale 100%](./static/images/specifications_1.png)

---
class: middle, center

## Does my dataset `comply`?

---
class: middle, center

## We need human and `machine-readable` specifications

.footnote[See also the [2017 TDWG presentation](https://speakerdeck.com/peterdesmet/defining-dataset-specifications-to-communicate-data-quality-characteristics) by Peter Desmet]

---
class: middle, center

![:scale 100%](./static/images/specifications_2.png)

---
class: middle, center

## We call them `whip` specifications

... be it a feather or a chain whip!

.footnote[https://github.com/inbo/whip]

---
class: middle, center

## pywhip

![:scale 100%](./static/images/pywhip_0.png)

.footnote[https://github.com/inbo/pywhip]

---
class: middle, center

## Input for pywhip

![:scale 100%](./static/images/pywhip_1.png)

---
class: middle, center

## Output of pywhip

![:scale 100%](./static/images/pywhip_2.png)

---
class: middle, center

## A reproducible workflow with a <i class="fa fa-check-square" aria-hidden="true"></i>

![:scale 85%](./static/images/workflow_7.png)

---
class: middle, center

# Thanks!

<br>

[<i class="fa fa-twitter"></i> @SVanHoey](https://twitter.com/svanhoey) [<i class="fa fa-github"></i> stijnvanhoey](https://github.com/inbo)

<br><br><br><br><br><br>

![:scale 25%](./static/images/CC-BY.svg)
