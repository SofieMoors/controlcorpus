# <p align = center> Witnessing Middle Dutch Textual Traditions. Diplomatic Transcriptions of *Dietsche Catoen*, *Scolastica*, and *Karel ende Elegast*</center> 

This dataset results from the research project *Constrained* (Sofie Moors) funded by the Research Foundation – Flanders (FWO), File Number 1182725N, and *Karel ende Elegast in Manuscript and Print* (Nicky Voorneveld), funded by the European Union under the Horizon Marie Skłodowska-Curie Doctoral Actions 2021, Project number 101072698 (REBPAF).

Cite this repository as: [![DOI](https://zenodo.org/badge/719645106.svg)](https://zenodo.org/doi/10.5281/zenodo.10245412)

This repository holds the code and data accompanying the following paper: Moors, S., Voorneveld, N. & Van Dalen-Oskam, K. (2025). "Witnessing Middle Dutch Textual Traditions. Diplomatic Transcriptions of *Dietsche Catoen*, *Scolastica*, and *Karel ende Elegast*" 

## ABSTRACT: 
We present a dataset of transcriptions of manuscripts and printed witnesses of the Middle Dutch texts *Dietsche Catoen*, *Rhymed Bible* or *Scolastica* (samples) and *Karel ende Elegast*. This open access dataset contains hyper-diplomatic transcriptions of these witnesses, amounting to a total of almost 29,000 verses. The data abides by the FAIR principles, is licensed under a CC-BY-SA license, and is available in multiple file formats. Due to its strictly diplomatic nature, this corpus is particularly suitable for research concerning, among others, textual stability, stemmatology and scribal profiling. 

**data**:
- `html`: html files with abbreviations expanded, html files with abbreviations unexpanded and extra folders with mvnhtml.css (the css view is optimized for macOS and iOS browsers)
- `mvn`: framework used (https://github.com/HuygensING/mvn-xml/tree/main/framework)
- `plain_txt`: text files generated from xml with markup applied (scripts > xml2txt.ipynb)
- `rich_txt`: raw text files, manually enriched with semantic markup: [legend](#legend-rich_txt)
- `viz`: timeline and pixelplot
- `xlsx`: synoptic presentation of all witnesses (abbreviations expanded) 
- `xml`: xml files generated from the rich_txt (scripts > txt2xml.ipynb) 

**scripts**:
- `txt2xml.ipynb`: code to convert `rich_txt` to `xml`
- `viz.ipynb`: code to create `viz`
- `xml2txt.ipynb`: code to convert `xml` to `plain_txt`
- `xml2xlsx.ipynb`: code to convert `xml` to `xlsx`


## LEGEND rich_txt:

| TRANSCRIPTION RICH_TXT |  EXAMPLE        |        INFORMATION               |        
|--------------------------|------------------------------|-----------------------------|
| &FOLIO_COLUMN&           | &2ra&, &112vb&               | New page and column          |                                            
| \_TEXTPART\_                | \_M1\_                         | New text part (M1, M2 or M3) |                                            
| _____                    | _____                        | End of text part             |                                            
| §STROPHE§                | §03§, §20§                   | New strophe                 |                                            
| <CHARACTER_HEIGHT>       | <O_3>m, \<D>e                 | Capital letter and height of letter |                                      
| {CHARACTER}              | {per}semier, dor{per}hede, or{con}de | Special abbreviatory glyphs (ꝫ, ꝑ, ꝰ, …) |                            
| CHARACTER(CHARACTER)     | en(de), co(ninc)             | Macron                      |                                            
| CHARACTER%CHARACTER%     | n%iet%, g%roe%t              | Abbreviation marked by superscript letter |                                                                              
| [...]                    | es [...], m[...]             | Damage gap                  |                                            
| \*CHARACTER*              | \*t*                          | Uncertain reading            |                                            
| CHARACTER[CHARACTER]     | s[er]e                       | Abbreviation marked by ʼ    |                                            
| Ø                        | Ø                            | Missing line (copyist error) |                                                                                 
| @CHARACHTER@             |  @gaen@ | Word crossed out |   
|«CHARACTER» |«koen» | Word added |
		

