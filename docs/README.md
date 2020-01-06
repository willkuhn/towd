## About the Project

**Dragonflies and damselflies (Odonata)** are highly skilled aerial acrobats, due largely to the intricacies of their most prominent features: their **wings**. These structures are both functional and beautiful: they provide extreme maneuverability and durability in a lightweight package, and they can be marked with bright color patterns and even iridescence! The structure and appearance of these wings provides a **rich source of information** about the evolutionary history, aerodynamic constraints, and behavior of a species.

The Targeted Odonata Wing Digitization (TOWD) Project is part of an [NSF-funded](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1564386&HistoricalAwards=false), multi-institutional effort to develop ODOMATIC, software for automatically identifying Odonata from images. Initiated in 2016, the TOWD Project aims to digitize the world's dragonfly and damselfly species, starting with the approx. **{{ site.data.stats.spp_comp.g }} North American species**. We are working to produce a **high-resolution imagery** of these species (including multiple males and females from each), partnering with several odonate collections, and building the most complete dataset of odonate wings ever compiled. Behind the scenes, we use **computer vision** to pull phenotypic information from our wings, which can be used for identification and comparative study.

The TOWD dataset will be used for **two main purposes**:
1. as training data to **expand the capabilities of [ODOMATIC](https://www.crossveins.com/research)** - an automatic species recognition system for dragonflies and damselflies, and
2. to **answer questions** about the flight strategies, mating behavior and other aspects of odonate evolutionary biology.

The TOWD Project's imagery dataset will be made available to the public on [OdonataCentral](https://www.odonatacentral.org/) via the [CyVerse](http://www.cyverse.org/) cyberinfrastructure, once the project is complete. Until then, you can [**view our progress**](#project-progress) below.

### How does digitization work?

We designed an inexpensive digitization setup that uses a commercially-available desktop scanner (connected to a computer) and custom-build paper 'frame' placed on the scanner glass to hold things in place and standardize our images. The image below is an example of the final product: one pair of wings is excised and scanned separately from the rest of the body, which is also scanned along with labels and a color standard and scale. Each item gets it's own 'window' in the frame and everything is imaged at once in one high-resolution scan.

{:.scan}
{% include image.html file="/assets/UA-000856.jpg" description="Example scan" %}

### What do we do with the scans?

Specimen scans are uploaded to our dataset on [Cyverse's BisQue](https://bisque.cyverse.org) - a powerful imaging platform that allows us to view them from a web browser or work with them from the backend via scripts using BisQue's API. It's at this point that one of the most exciting parts of the project takes place behind the scenes, governed by [scripts](#project-on-github). Our specimen inventory is updated periodically by a script that reads barcodes and labels from the latest scans and checks them against collection databases to get species names and locality information associated with them. Another script detects the wings in each image and automatically measures morphometric properties of each wing (area, length, width, etc.), and also calculates information about its appearance and texture. We can these use these data to make comparisons among species or to update our ODOMATIC species recognition model, using machine learning.

### Acknowledgement of NSF Support
This material is based upon work supported by the National Science Foundation under Grant No. 1564386. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.

***

## Project progress

Our goal is to image at least 10 males and 10 females from each of the {{ site.data.stats.spp_comp.g }} dragonfly and damselfly species in Canada and the US. The progress of this ambitious endeavor (as of {{ site.data.stats.last_update }}) is illustrated in two forms below.

### North American progress (visual):

{% include image.html file="/assets/Scanning progress - North American Odonata.png" description="Represented here are all odonate species from US and Canada. Bars represent species; clusters of bars are genera (sorted alphabetically); rows are families; progress bars are the number of ♀ (red) and ♂ (blue) scans we've made out of 10 for each species." %}

### North American progress (tabular):

{% include quick_stats_table.html %}

***

## Who is the TOWD Project?

### Meet Our Team

#### Dr. Jessica L. Ware, PI ([website](https://www.jessicalwarelab.com/))
Jessica is an Associate Professor at Rutgers University-Newark and heads the Insect Systematics (IS) Lab there, where she and her students explore the evolutionary history of Odonata (dragonflies and damselflies) as well as Dictyoptera (cockroaches, termites, and mantises). She leads the TOWD digitization and research efforts at Rutgers.

#### Dr. John C. Abbott, co-PI ([website](https://almnh.ua.edu/abbott.html))
John is an odonatologist and the Director of Museum Research & Collections at the Alabama Museum of Natural History in Tuscaloosa. He leads the TOWD digitization efforts at ALMNH.

#### Dr. Gareth Russell, co-PI ([website](https://sites.google.com/a/njit.edu/russell-lab/))
Gareth is an Associate Professor at the New Jersey Institute of Technology and plays an advisory role in the TOWD Project.

#### Dr. William R. Kuhn, senior personnel ([website](https://crossveins.com))
Will is a graduate of the IS Lab and is now an NSF Postdoctoral Fellow at the University of Tennessee in Knoxville. The TOWD project is an extension of his dissertation work, in which he digitized a small set of Odonata and developed ODOMATIC. He manages the data workflow for TOWD, as well as this website.

#### Dr. Kimberly N Russell, senior personnel ([website](https://kimberlynrussell.weebly.com/))
Kim is an Assistant Professor at Rutgers University-New Brunswick and plays an advisory role in the TOWD Project.

#### Dr. Michael L May, senior personnel ([website](https://entomology.rutgers.edu/personnel/michael-may.html))
Mike is a retired Professor from Rutgers University-New Brunswick and plays an advisory role in the TOWD Project.

#### Dr. Melissa Sanchez Herrera, postdoc ([website](https://www.polythore.com/))
Also a graduate of the IS Lab, Melissa worked as a postdoc under the TOWD Project in 2017. There she helped get the Project up and running -- developing our digitization protocol, beginning our effort to scan Odonata from several collections with a team of undergraduate students, and much more! She continues to collaborate with us from her new/old home in Bogotá, Colombia.

#### Dr. Dirk Gassmann, postdoc ([website](https://www.jessicalwarelab.com/postdoctoral))
Dirk worked as a postdoc under the TOWD project. He managed a team of undergraduate students at Rutgers, continuing our scanning effort there. Dirk worked to develop additional odonate datasets, seeking to answer questions about flight strategies among dragonflies.

#### Dr. Manpreet Kohli, senior personnel ([website](https://manpreetkohli.me/))
Manpreet is a recent graduate of the IS Lab and has played an advisory role for the TOWD Project.

### Odonata Collection Partners

Our work couldn't be done without the dragonfly and damselfly specimens to digitize. We've partnered with several Odonata collections in North America. We'd like to thank our partners for allowing us to work with their collections!

- Insect Systematic Lab Collection at Rutgers University-Newark (NJ)
- Mike May Collection (New Brunswick, NJ)
- John Abbott Collection (Tuscaloosa, AL)
- Rosser W. Garrison Collection (Sacramento, CA)

***

## Outputs

### Presentations

Kuhn, WR, JL Ware, JC Abbott, M Sanchez-Herrera, D Gassmann (2019) Automatically measuring dragonfly wings: an update on the Targeted Odonata Wing Digitization (TOWD) project. International Congress of Odonatology, Austin, TX.

Ware, JL, WR Kuhn, JC Abbott (2019) Using specimens from the past to understand the living world through digitization. Eastern Branch Meeting of the Entomological Society of America, Blackburg, VA. ([slides pdf and related talks](https://www.idigbio.org/wiki/index.php/Digital_Future_of_Entomology_at_Eastern_Branch_EntSoc_2019))

Gassmann, D, J Ware, W Kuhn, JC Abbott, M Sanchez (2018) The Targeted Odonata Wing Digitization (TOWD) project: creating a unique resource for studying wing evolution in dragonflies (Odonata). Entomological Society of America Annual Meeting, Vancouver, BC, Canada.

Kuhn, WR, JL Ware, JC Abbott, M Sanchez-Herrera, D Gassmann (2017) Automatic dragonfly identification with Odomatic and the Targeted Odonata Wing Digitization (TOWD) project. International Congress Odonatology, Cambridge, UK.

Kuhn, WR, G Russell, J Ware (2016) Ode-omatic ID: A system for automatically identifying dragonflies and damselflies from wings. XXV International Congress Entomology, Orlando, FL.

### Posters

Elmonier, A, D Gassmann, WR Kuhn, J Ware (2018) The relationship between wing color pattern, wing area, and wing weight in *Celithemis* dragonflies based on the TOWD image database. 10th Annual GS-LSAMP Research Conference, Rutgers University-Newark, NJ. [pdf](assets/Ahmed_poster.pdf)

### Publications

Coming soon!

***

## Resources

- [TOWD Project image library (on CyVerse BisQue)](https://bisque.cyverse.org/client_service/view?resource=https://bisque.cyverse.org/data_service/00-F7qU3mVyCvyoTqPzrbiHZA)
- [printable scanning frame](/resources/TOWD scanning frame v2_0.pdf)
- [printable template for foamboard cutouts](/resources/TOWD foamboard cutouts template.pdf) (part of scanning process)
- [TOWD digitization instructions](/resources/TOWD digitization protocol.pdf) on Windows or Linux, using GIMP
- [TOWD digitization instructions](/resources/TOWD digitization protocol - Mac, no GIMP.pdf) on Mac OS
- [color standard](https://www.bhphotovideo.com/c/product/714596-REG/Tiffen_EK1527654T_Q_13_Color_Separation_Guide.html) - Tiffen Q-13 Color Separation Guide (Small)

### Project on GitHub

The behind-the-scene scripts that run the data workflow of this project are publicly available on [GitHub](https://github.com/willkuhn/towd-wing-scanning-project).
