---
layout: home
---

{% assign cacheBust = site.time | date:'?v=%s' %}
![Image]({{ "/images/AstraBeamLED-3D_blender_top_angled.png" | relative_url | append: cacheBust }}){: width="400" }

OSRAM OSTAR® Stage Light PCB
LE RTDUW S2WN

High Power 40W RGBCY LED PCB with direct heatsink copper base.


[![CI](https://github.com/LiveLeds/AstraBeamLED/actions/workflows/ci.yml/badge.svg)](https://github.com/LiveLeds/AstraBeamLED/actions/workflows/ci.yml)
## Table of contents

- [Table of contents](#table-of-contents)
  - [Render Top Angled](#render-top-angled)
  - [Render Top](#render-top)
  - [Render Bottom](#render-bottom)
  - [Interactive BOM](#interactive-bom)
  - [BOM](#bom)
  - [KiCad Revision Inspector (KiRI)](#kicad-revision-inspector-kiri)
    - [Dark](#dark)
    - [Light](#light)
  - [Schematic](#schematic)
    - [Dark](#dark-1)
    - [Monochromatic](#monochromatic)
    - [Light](#light-1)
  - [Assembly](#assembly)
    - [Dark](#dark-2)
    - [Light](#light-2)
  - [3D Step](#3d-step)
  - [Downloads](#downloads)
    - [JLCPCB](#jlcpcb)
    - [Eurocircuits](#eurocircuits)
- [Report](#report)
    - [ERC](#erc)
    - [DRC](#drc)
- [Credits](#credits)

### Render Top Angled

![Image]({{ "/images/AstraBeamLED-3D_blender_top_angled.png" | relative_url | append: cacheBust }})

### Render Top

![Image]({{ "/images/AstraBeamLED-3D_blender_top.png" | relative_url | append: cacheBust }})

### Render Bottom

![Image]({{ "/images/AstraBeamLED-3D_blender_bottom.png" | relative_url | append: cacheBust }})

### Interactive BOM

Easily check component locations by hovering over a specific component.

[IBOM HTML]({{ "/export/AstraBeamLED-ibom.html" | relative_url | append: cacheBust }})

### BOM

All components with Values, References, Sheetpath and Links to the datasheet.

[BOM HTML]({{ "/export/AstraBeamLED-bom.html" | relative_url | append: cacheBust }})

### KiCad Revision Inspector (KiRI)

KiCad Revision Inspector (KiRI) is a tool for comparing different versions of KiCad projects. It exports project revisions to SVG format for visual comparison using an onion skin view. This helps identify changes and errors in PCB designs. KiRI also includes a command line interface for generating viewable artifacts in any web browser.

View the PCB / Schematic in an interactive way, pan and zoom to see the details.

#### Dark

- [KiRi Dark]({{ "/KiRiDark/index.html" | relative_url | append: cacheBust }})

#### Light

- [KiRi Light]({{ "/KiRiLight/index.html" | relative_url | append: cacheBust }})

### Schematic

#### Dark

- [Schematic Dark PDF]({{ "/documents/AstraBeamLED-schematic-dark.pdf" | relative_url | append: cacheBust }})

#### Monochromatic

- [Schematic Monochromatic PDF]({{ "/documents/AstraBeamLED-schematic-mono.pdf" | relative_url | append: cacheBust }})

#### Light

- [Schematic Light PDF]({{ "/documents/AstraBeamLED-schematic-default.pdf" | relative_url | append: cacheBust }})

### Assembly

#### Dark

- [PCB Dark PDF]({{ "/documents/AstraBeamLED-pcb-dark.pdf" | relative_url | append: cacheBust }})

#### Light

- [PCB Light PDF]({{ "/documents/AstraBeamLED-pcb-light.pdf" | relative_url | append: cacheBust }})

### 3D Step

- [3D Step]({{ "/AstraBeamLED-3D.step" | relative_url | append: cacheBust }})


### Downloads

#### JLCPCB

- [JLCPCB Zip]({{ "export/AstraBeamLED-JLCPCB.zip" | relative_url | append: cacheBust }})
- [JLCPCB BOM CSV]({{ "export/AstraBeamLED_bom_jlc.csv" | relative_url | append: cacheBust }})
- [JLCPCB CPL CSV]({{ "export/AstraBeamLED_cpl_jlc.csv" | relative_url | append: cacheBust }})

#### Eurocircuits

- [Eurocircuits Zip]({{ "export/AstraBeamLED-Eurocircuits.zip" | relative_url | append: cacheBust }})
- [Eurocircuits BOM CSV]({{ "export/AstraBeamLED_bom_Eurocircuits.csv" | relative_url | append: cacheBust }})
- [Eurocircuits CPL CSV]({{ "export/AstraBeamLED_cpl_Eurocircuits.csv" | relative_url | append: cacheBust }})
  
## Report

#### ERC

{% include_relative erc_validation.md %}

#### DRC

{% include_relative drc_validation.md %}

{% include_relative AstraBeamLED-report.md %}


## Credits

[KiCad EDA](https://www.kicad.org)

[KiBot](https://github.com/INTI-CMNB/KiBot)

[Amulet - Inspiration for awesome schematic and PCB](https://github.com/EPFLXplore/XRE_LeggedRobot_HW)

Sorry if I am forgetting someone, I used lots of references and tips from all over the place.