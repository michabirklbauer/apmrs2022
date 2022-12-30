# Identifying Crosslinks in MS2-MS3-based Workflows with MS Annika

Short talk presentation for [APMRS 2022](https://www.apma.at/2022/02/14/scp-apmrs-2022/) presented on the 13th of September 2022 in Vienna.

## Abstract

**Identifying Crosslinks in MS2-MS3-based Workflows with MS Annika**

Micha Johannes Birklbauer [1], Manuel Matzinger [2], Fränze Müller [2], Karl Mechtler [2, 3, 4], Viktoria Dorfer [1]

[1] University of Applied Sciences Upper Austria, Bioinformatics Research Group, Softwarepark 11, 4232 Hagenberg, Austria  
[2] Institute of Molecular Pathology (IMP), Vienna BioCenter (VBC), Campus-Vienna-Biocenter 1, 1030 Vienna, Austria  
[3] Institute of Molecular Biotechnology (IMBA), Austrian Academy of Sciences, Vienna BioCenter (VBC), Dr. Bohr-Gasse 3, 1030 Vienna, Austria  
[4] Gregor Mendel Institute (GMI), Austrian Academy of Sciences, Vienna BioCenter (VBC), Dr. Bohr-Gasse 3, 1030 Vienna, Austria

**Keywords:** cross-linking, bioinformatics, search engine, MS3, XL-MS, protein-protein-interaction, PPI

**Introduction**

Cross-linking mass spectrometry has become a powerful tool to identify protein-protein interactions and to gain insight into the structures of proteins in living cells, tissues, or organelles. Over the past few decades this field has constantly evolved and the development of new cross-linkers, enrichment strategies and data acquisition methods for mass spectrometry led to the establishment of numerous new software tools specifically for the analysis and interpretation of cross-linking data. We previously presented on of these tools: MS Annika, a cross-linking search engine which can accurately identify cross-linked peptides in MS2 spectra from a variety of different cleavable cross-linkers.

**Methods & Results**

In our newest version of MS Annika, we are introducing a new feature which enables processing of data from MS2-MS3-based approaches and identification of peptides from MS3 spectra. In the new MS2-MS3 workflow MS Annika matches each MS3 spectrum to the corresponding doublet peak of the precursor MS2 spectrum to identify the crosslink modification and classify every MS3 spectrum as either an alpha or beta peptide spectrum. Subsequently using this information all MS3 spectra are adjusted for search and MS Amanda, our in-house developed peptide search engine, is used to identify the cross-linked alpha and beta peptides. Peptides that are identified in the MS2 and one or more MS3 spectra are re-scored with a novel scoring function to reflect the increased confidence. The found cross-links are validated by estimating the false discovery rate (FDR) using a target-decoy approach and are reported at 5% and 1% FDR confidence levels. We evaluated the MS3-capabilities of MS Annika on two different datasets of synthetic peptides and compared it to XlinkX and MaXLinker, two other crosslinking search engines that support MS3 identification. The results show that MS Annika outperforms both tools in both datasets in terms of total number of unique crosslinks found while simultaneously yielding less false-positives and therefore better FDR estimates.

## Contact

- [micha.birklbauer@gmail.com](mailto:micha.birklbauer@gmail.com)
