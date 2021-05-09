---
design:
  columns: "1"
  spacing:
    padding: [50px, 0px, 20px , 20px]

---

# Research

Inside our cells, genetic information is encoded on meter-long chromosomes with hundreds-of-millions of nucleotides organized inside micron-scale cell nuclei. 

Our goal is to identify and answer the fundamental questions in genome biology posed by this immense range of scales. These include:
- _How do molecular interactions between proteins organize micron-long chromosomes?_  
- _Which DNA sequences specify when & how this organization occurs?_  
- _How does genome oranization influence communication between DNA regulatory elements?_  

We believe the answers to these questions are key links for connecting molecular processes and macroscopic phenotypes.

As a computational group, our approach involves building quantitative models that can bridge the gap between (i) individual nucleotides and full genomes, (ii) molecular-scale mechanisms and genome-wide consequences, and (iii) develop tools to synthesize and analyze rapdily growing quantities and modalities of genomic data. A key aspect of our approach involves close collaborations with experimental and computational colleagues. 
  
Two projects that illustrate our approach are higlighted below, with links to key papers, review articles, and code. The first project asks which DNA sequences specify genome organization and makes use of convolutional neural networks. The second aims to understand mechanisms of 3D genome organization, and makes use of polymer simulations.

###### DNA sequence determinants of 3D genome folding  

<img src="/media/akita-minimal-05-06-2021.png" alt="akita-fig"
    title="akita-fig" style="float: right;" width="450px" /> 

To connect the impact of individual DNA nucelotides with 3D genome folding, we leveraged recent progress in designing and training convolutional neural networks. We devleoped a convolutional neural network, [Akita](https://github.com/calico/basenji/tree/master/manuscripts/akita), that learns accurate representations of genome folding from DNA sequence ([paper](https://www.nature.com/articles/s41592-020-0958-x.epdf?sharing_token=BlG7pTRCDh28fnOS-Xo2O9RgN0jAjWel9jnR3ZoTv0MnfQPOPiHQ2lAYRF462xp4UslZdaa6D1Ky97gz1cIuf-UMnZeGKcMi7TWxVkbSlpzVtfdKXKO657MHJRoDSaIX-CO3Zeuz8eNGla7prHZv2BQrJv1-90deyQhVNsRsvas%3D), [github](https://github.com/calico/basenji/tree/master/manuscripts/akita), [poster & talk](https://zenodo.org/record/3942645#.YIYIfBNKjlw)). The network has a ‘trunk’ which pools input sequences to 2048bp resolution and shares information across the sequence with dilated residual convolutions. This is followed by a ‘head’ which transforms from a latent space of 1D profiles to 2D maps of a megabase-by-megabase region. While computationally intensive to fit, trained models can be used to make hundreds of predictions per second, enabling _in silico_ mutagenesis at scales beyond foreseeable experimental capabilities. We are excited about pursuing applications of this model as well as developing new network architectures and training strategies to make improved predictions. Applications we are excited about include those relating to: (i) evolution, (ii) _de novo_ variant interpretation, and (iii) DNA sequence design _in silico_.


###### Loop extrusion as a mechanism of genome organization  

<img src="/media/extrusion-cartoon-adapted-05-02-2021.png" alt="extrusion-fig" title="extrusion-fig" style="float: left;" width="425px" caption="asdfasd" />  

To understand how 3D folding patterns emerge in mammalian interphase Hi-C maps, we implemented and tested a range of possible mechanisms using polymer simluations. We found that the mechanism of loop extrusion limited by barriers could recapitulate many features of experimental data ([paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4889513/), [review article](https://pubmed.ncbi.nlm.nih.gov/29728444/)). This mechanism involves processive molecular machines that dynamically enlarge chromatin loops as they translocate hundreds of thousands of nucleotides along the chromatin fiber. Extruder translocation continues unless extruders become stalled at a barrier, or against another extruder, until they dissociate from the chromatin fiber. Spurred by these results, we collaborated with experimentalists to better understand the molecular basis for how barriers halt extrusion in interphase ([paper](https://www.nature.com/articles/s41467-020-19283-x)), as well as how extrusion might operate to organize chromosomes in meiosis ([paper](https://www.nature.com/articles/s41467-019-12629-0)). We are excited about developing new models to understand: (i) how loop extrusion can enable communication between enhancers and promoters, (ii) when and how regulators modulate loop extrusion dynamics, (iii) rules governing the encounters between extruders and barriers, (iv) the interplay between loop extrusion and other mechanisms of genome organization (e.g. heterochromatin phase separation in interphase, or synaptonemal complex assembly in meiosis).

###### See [publications](../publication) and [resources](../resources) for more information. 

