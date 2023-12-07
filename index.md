---
title       : "Multi-locus phylogenetics"
subtitle    : "BNS-2002: Genes, Development, and Evolution"
author      : Dr Axel Barlow
job         : "email: a.barlow@bangor.ac.uk"
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn      # {zenburn, tomorrow, solarized-dark, ...}
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {selfcontained, standalone, draft}
knit        : slidify::knit2slides
logo        : LA_Full_colour_reversed.svg
biglogo     : A1_FullColour.svg
assets      : {assets: ../../assets}
license     : by-nc-sa

---



<!-- adding bold and italic options -->
<style>
em {
  font-style: italic
}
strong {
  font-weight: bold;
}
</style>

## Phylogenetics and population genetics lectures

- Key concepts and Single locus phylogenetics
- **Multi-locus phylogenetics**
  - **Theory**
  - **Methods**
  - **Discoveries**
- Population structure
- Conservation genetics

--- .segue .dark 

## Multi-locus phylogenetics - theory

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort1.svg" alt="plot of chunk unnamed-chunk-1" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort2.svg" alt="plot of chunk unnamed-chunk-2" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort3.svg" alt="plot of chunk unnamed-chunk-3" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort4.svg" alt="plot of chunk unnamed-chunk-4" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort5.svg" alt="plot of chunk unnamed-chunk-5" width="100%" style="display: block; margin: auto;" />

---

## Lineage sorting summary

- Drift sorts the lineages into clades
- This takes time, we can't detect the divergence immediately
- We go through stages of incomplete/complete monophyly
- incomplete to complete lineage sorting
- lineage sorting is faster when the population size is small (= more drift)
- Mutation builds upon the clades, monophyly is retained [unless there is gene flow]
- ILS can be a real problem for inferring relationships, especially in large populaitons with recent divergence events

--- @vcenter bg:white

<img src="./assets/img/istockphoto-840934838-612x612.jpg" alt="plot of chunk unnamed-chunk-6" width="60%" style="display: block; margin: auto;" />

--- 

## Relying on a single locus tree could be misleading

- Incomplete lineage sorting could mean that clades do not correspond to species/populations
- Old divergence with small populations less likely to cause problems
- But no way of easily predicting/testing this from a single tree
- Also may fail to account for sex-specific differences (e.g. mtDNA and Y chromosome)

### Solution: multiple loci

- Increased statistical confidence
- Can detect sex-specific differences
- Can also quantify ILS (says something about pop size and divergence time)
- Potential to study **gene flow** [more later]

--- .segue .dark 

## Multi-locus phylogenetics - methods

---

## Getting the data

### Modest number of loci

- Several PCRs
- Transcriptomes
- Hybridisation capture
  - Ultraconserved elements
  - Exomes

### Whole genomes

- de novo assembly and whole genome alignment [hard]
- shotgun whole genome resequencing

---

## Shotgun whole genome sequencing

<img src="./assets/img/aDNA_seq.svg" alt="plot of chunk unnamed-chunk-7" width="95%" style="display: block; margin: auto;" />

---

## Mapping to reference genome assembly

- Whole sample DNA is sequenced in short reads
- These are "mapped" to a reference whole genome sequence based on similarity
  - Nuclear chromosomes
  - Mitochondrial/chloroplast genomes
  - Potentially other genomes too (bacteria, pathogens, etc.)
  - Around £150-200 for a 2-3Gb genome, currently

<img src="./assets/img/pseudohap.svg" alt="plot of chunk unnamed-chunk-8" width="95%" style="display: block; margin: auto;" />

---

## Data analysis

### Separate loci

- Analyse each locus separately, look for concordant patterns
- Combine all together (concatenation)
- More complex models, e.g. multispecies coalescent

### Whole genome

- Concatenation easy
- Divide chromosomes into non-overlapping chunks (very approximate)
  - not based on actual recombination points
  - mostly the diploid alleles are not phased
  - in practise works very well
- More sophisticated methods that identify the true breakpoints between loci 

--- .segue .dark 

## Multi-locus phylogenetics - discoveries

--- &twocol

## Brown bear and polar bears

*** =left

<img src="./assets/img/arctos_mt.svg" alt="plot of chunk unnamed-chunk-9" width="100%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/arctos_map.svg" alt="plot of chunk unnamed-chunk-10" width="100%" style="display: block; margin: auto;" />

- Brown bears not monophyletic
- Divergence time ~120 Ka
- Incomplete lineage sorting (result of recent speciation)?
- Something else?
- Multiple divergent brown bear clades
- Evidence of glacial refugia

--- bg:white

## Brown bear and polar bear Y chromosome

<img src="./assets/img/arctos_y.svg" alt="plot of chunk unnamed-chunk-11" width="100%" style="display: block; margin: auto;" />

--- &twocol bg:white

## Brown bear and polar bear autosomes

*** =left

<img src="./assets/img/arctos_auto.svg" alt="plot of chunk unnamed-chunk-12" width="80%" style="display: block; margin: auto;" />

*** =right

- mtDNA suggests recent speciation and brown bear glacial refugia
- Y chromosome suggests species monophyly, no evidence of brown bear refugia
- Autosomes show species monophyly, and that the species are OLD (latest estimates, 1 million years)

### Explanation

- The 2 species are old and distinct
- Males move about more than females
- More recent mtDNA divergence suggests **gene flow**

--- .segue .dark 

## Detecting gene flow

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary1.svg" alt="plot of chunk unnamed-chunk-13" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary2.svg" alt="plot of chunk unnamed-chunk-14" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary3.svg" alt="plot of chunk unnamed-chunk-15" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary4.svg" alt="plot of chunk unnamed-chunk-16" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary5.svg" alt="plot of chunk unnamed-chunk-17" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## What if lineage sorting is incomplete?

---

## Speciation with incomplete lineage sorting

<img src="./assets/img/beary1.svg" alt="plot of chunk unnamed-chunk-18" width="100%" style="display: block; margin: auto;" />

---

## Speciation with incomplete lineage sorting

<img src="./assets/img/beary2.svg" alt="plot of chunk unnamed-chunk-19" width="100%" style="display: block; margin: auto;" />

---

## Speciation with incomplete lineage sorting

<img src="./assets/img/ils3.svg" alt="plot of chunk unnamed-chunk-20" width="100%" style="display: block; margin: auto;" />

---

## Speciation with incomplete lineage sorting

<img src="./assets/img/ils4.svg" alt="plot of chunk unnamed-chunk-21" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## Or...

---

## Speciation with incomplete lineage sorting

<img src="./assets/img/ils3.svg" alt="plot of chunk unnamed-chunk-22" width="100%" style="display: block; margin: auto;" />

---

## Speciation with incomplete lineage sorting

<img src="./assets/img/ils5.svg" alt="plot of chunk unnamed-chunk-23" width="100%" style="display: block; margin: auto;" />

---

## Simulator

<iframe src = 'https://www.whfreeman.com/BrainHoney/Resource/6716/SitebuilderUploads/Hillis2e/Student%20Resources/Animated%20Tutorials/pol2e_at_1502_genetic_drift_simulation/pol2e_at_1502_genetic_drift_simulation.html' height='600px'></iframe>

---

## Summary

- [Note these a just some of the many outcomes you could imagine]
- The danger zone is when alleles fail to reach fixation early in the speciation process
- i.e. prior to brown bear population divergence in the example
- Because there is no selection for specific alleles, the process is random
- Either brown bear population may end up grouping with the polar bears

### What can you predict about the relative frequencies of these alternatives?

---

## Expected tree frequecies under ILS?

<img src="./assets/img/freq.svg" alt="plot of chunk unnamed-chunk-24" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## What about gene flow?

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary5.svg" alt="plot of chunk unnamed-chunk-25" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/bearyG.svg" alt="plot of chunk unnamed-chunk-26" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/bearyG2.svg" alt="plot of chunk unnamed-chunk-27" width="100%" style="display: block; margin: auto;" />

---

## Expected tree frequencies with gene flow?

<img src="./assets/img/flow.svg" alt="plot of chunk unnamed-chunk-28" width="100%" style="display: block; margin: auto;" />

---

## Summary

- An inbalance in the non-species tree topologies provides evidence of gene flow
- Only works if you have sequenced a LOT of loci (whole genomes)
- Can detect very ancient events
- And sex-biases (e.g. X chromosome vs. autosome)
- Sometimes based on SNPs (D statistics, F-ratio statistics), essentially the same
- Revealed many examples of gene flow in the past decade

--- &twocol

## Brown bear and polar bears

*** =left

<img src="./assets/img/arctos_mt.svg" alt="plot of chunk unnamed-chunk-29" width="100%" style="display: block; margin: auto;" />

*** =right

**Nuclear genomes, 100 kb windows**

<img src="./assets/img/abc.svg" alt="plot of chunk unnamed-chunk-30" width="80%" style="display: block; margin: auto;" />

---

## Brown bear and polar bear reading

<embed src="./assets/img/2015-Genomic_evidence_of_geographically_widespread_effect_of_gene_flow_from_polar_bears_into_brown_bears..pdf" title="plot of chunk unnamed-chunk-31" width="100%" height="500" type="application/pdf" />

---

## Brown bear and polar bear reading

<embed src="./assets/img/2014-Brown_and_polar_bear_y_chromosomes_reveal_extensive_male-biased_gene_flow_within_brother_lineages.pdf" title="plot of chunk unnamed-chunk-32" width="100%" height="500" type="application/pdf" />

--- &twocol

## Cave bears and brown bears

*** =left

- Cave bears are sister lineage to brown bears and polar bears
- Giant vegan bears
- Extinct ~25 Ka
- Lived alongside brown bears for most of their evolutionary history

*** =right

<img src="./assets/img/kudarensis.png" alt="plot of chunk unnamed-chunk-33" width="100%" style="display: block; margin: auto;" />

<img src="./assets/img/Ursus_spelaeus_Sergiodlarosa.jpg" alt="plot of chunk unnamed-chunk-34" width="90%" style="display: block; margin: auto;" />

--- &twocol

## Cave bears and brown bears

*** =left

**Nuclear genomes, 25 kb windows**

<img src="./assets/img/cave_freq.svg" alt="plot of chunk unnamed-chunk-35" width="80%" style="display: block; margin: auto;" />
*** =right

<img src="./assets/img/kudarensis.png" alt="plot of chunk unnamed-chunk-36" width="100%" style="display: block; margin: auto;" />

<img src="./assets/img/Ursus_spelaeus_Sergiodlarosa.jpg" alt="plot of chunk unnamed-chunk-37" width="90%" style="display: block; margin: auto;" />

---

## Cave bear reading

<embed src="./assets/img/Barlow et al. - 2018 - Partial genomic survival of cave bears in living brown bears.pdf" title="plot of chunk unnamed-chunk-38" width="100%" height="500" type="application/pdf" />

--- &twocol

## Neanderthals and anatomically modern humans

*** =left

- Extinct population of humans
- Extinct ~40 Ka
- Basically a human (many morphological characters overlapping)
- Advanced culture, hunting technology, art, etc.
- Major dispersal of anatomically modern humans 70-50 Ka
- Population replacement or admixture?

*** =right

<img src="./assets/img/neanderthal_woman-4x3.jpg" alt="plot of chunk unnamed-chunk-39" width="100%" style="display: block; margin: auto;" />

--- &twocol

## Neanderthals and anatomically modern humans

*** =left

<img src="./assets/img/neander.svg" alt="plot of chunk unnamed-chunk-40" width="100%" style="display: block; margin: auto;" />

[SNP based analysis, but essentially the same]

*** =right

<img src="./assets/img/neanderthal_woman-4x3.jpg" alt="plot of chunk unnamed-chunk-41" width="100%" style="display: block; margin: auto;" />

---

## Neanderthal reading

<embed src="./assets/img/2010-A_draft_sequence_of_the_Neandertal_genome..pdf" title="plot of chunk unnamed-chunk-42" width="100%" height="500" type="application/pdf" />

--- &twocol

## Bengal cat

*** =left

<img src="./assets/img/far.jpg" alt="plot of chunk unnamed-chunk-43" width="90%" style="display: block; margin: auto;" />

<img src="./assets/img/Asian-Leopard-Cat-Prionailurus-bengalensis-758x432.webp" alt="plot of chunk unnamed-chunk-44" width="90%" style="display: block; margin: auto;" />

*** =right

- Hybrid domestic cat/*Prionailurus bengalensis*
- F1 hybrids backcrossed 6+ generations
- Selection for coat pattern and other introgressed traits
- A framework to better understand the process and refine methodologies???

<img src="./assets/img/prio.svg" alt="plot of chunk unnamed-chunk-45" width="80%" style="display: block; margin: auto;" />

--- .segue .dark 

## MSc project?

--- &thankyou

## Next time

**Population structure**

