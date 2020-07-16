PSAMM model collection
======================

This is a collection of published GEMs that have been converted to the YAML
format used by [PSAMM](https://github.com/zhanglab/psamm), using the
[psamm-import tool](https://github.com/zhanglab/psamm-import). These model
files serve as an easy way for people interested in PSAMM to get started on
working with these models.

The models in this repository were originally used for the analysis performed
in the following publication but the files here have been updated since the
publication to follow more recent conventions of the PSAMM software. To
access the model files as they were originally used, please use the
[archived-models branch](https://github.com/zhanglab/psamm-model-collection/tree/archived-models).

```
Steffensen JL, Dufault-Thompson K, Zhang Y. PSAMM: A Portable System for the
Analysis of Metabolic Models. PLOS Comput Biol. Public Library of Science;
2016;12: e1004732. 10.1371/journal.pcbi.1004732.
```

The original files for the models were obtained from the publications
referenced in the tables below (unless otherwise noted). During the
analysis of the models, some models had issues corrected which are
summarized in the first table below. The table also references the Git commits
that document the _exact_ changes that were made to the model files.

**No files in this repository are original model publications. To
obtain the original model files please consult the original publications
listed below.**

The collection of models is split into three sections:

- [**sbml**](sbml): Models that have been loaded as SBML files using the _sbml_
  loader in _psamm-import_.
- [**excel**](excel): Models that have been loaded using a model-specific Excel
  file loader in _psamm-import_.
- [**matlab**](matlab): Models that have been loaded from MATLAB data files
  using the
  [PSAMM MATLAB importer](https://github.com/zhanglab/psamm-import-matlab).

Model Format Curations
-----------------

|Model|Correction(s)|Commit(s)|
|-----|----------|-------|
|[iJN746](sbml/iJN746)     | Corrected compound references to cardiolipins in biomass reaction to refer to cardiolipins in the periplasm. |[7d68a62](https://github.com/zhanglab/psamm-model-collection/commit/7d68a6236faf5835229971cbc84cc2eab36ca1fa) |
|[iKF1028](sbml/iKF1028)   | Corrected stoichiometric balances. | [8791efa](https://github.com/zhanglab/psamm-model-collection/commit/8791efa58d0b01a06384b03ce11a6fcbc03fe8c3) |
|[iMA871](sbml/iMA871)     | 1. Added missing exchange reaction for BIOMASS compound and removed duplicate compounds in a number of reactions. 2. Added biomass reaction definition. | [1. b10e858, ](https://github.com/zhanglab/psamm-model-collection/commit/b10e85808287982564dcd0cb0b9290104ce39b4f) [2. b4249ed](https://github.com/zhanglab/psamm-model-collection/commit/b4249ed9d3a6a973e9b9c0195dfeaa4f6127e353) |
|[iRsp1095](sbml/iRsp1095) | 1. Changed medium for growth based on medium description in [Imam et al. 2011] (https://doi.org/10.1186/1752-0509-5-116). 2. Made all lower exchange bounds zero. 3. Marked zeromass compounds. 4. Added biomass reaction definition. | [1. 3340d7a, ](https://github.com/zhanglab/psamm-model-collection/commit/3340d7a476485a6e22f77a0561a803b4281d2615) [2. 15f48dc, ](https://github.com/zhanglab/psamm-model-collection/commit/15f48dc29695144da9a7c227a398170a65686e73) [3. 405ee9d, ](https://github.com/zhanglab/psamm-model-collection/commit/405ee9dda1d4e6cc74e339c8e76a788cb5d86656) [4. b4249ed](https://github.com/zhanglab/psamm-model-collection/commit/b4249ed9d3a6a973e9b9c0195dfeaa4f6127e353) |
|[iSyn731](sbml/iSyn731)   | Updated to new model from http://www.maranasgroup.com/models.htm downloaded on September 9, 2015. | [ca39f98](https://github.com/zhanglab/psamm-model-collection/commit/ca39f98172275718bdbc369c53015b71aec91e70) |
|[RECON1](sbml/RECON1)     | Fixed stoichiometric consistency. | [f72da25](https://github.com/zhanglab/psamm-model-collection/commit/f72da25d9a9e0e6ac319d3ebb566764bb1733cf5) |
|[RECON2](sbml/recon2)     | Fixed stoichiometric consistency. | [5671060](https://github.com/zhanglab/psamm-model-collection/commit/5671060606674cec61141f71dbe0d9d545e149dc) |
|[AORYZAE_COBRA](sbml/AORYZAE_COBRA)     | 1. Allowed essential compounds in medium. 2. Added biomass reaction definition. | [1. 134968f, ](https://github.com/zhanglab/psamm-model-collection/commit/134968fac483e57d9b2c7701e77d276900703728) [2. b4249ed](https://github.com/zhanglab/psamm-model-collection/commit/b4249ed9d3a6a973e9b9c0195dfeaa4f6127e353) |
|[iCce806](sbml/iCce806)   | 1. Marked zeromass compounds. 2. Added biomass reaction definition. | [1. 405ee9d, ](https://github.com/zhanglab/psamm-model-collection/commit/405ee9dda1d4e6cc74e339c8e76a788cb5d86656) [2. b4249ed](https://github.com/zhanglab/psamm-model-collection/commit/b4249ed9d3a6a973e9b9c0195dfeaa4f6127e353) |
|[iRC1080](sbml/iRC1080)   | 1. Marked zeromass compounds. 2. Added biomass reaction definition. | [1. 405ee9d, ](https://github.com/zhanglab/psamm-model-collection/commit/405ee9dda1d4e6cc74e339c8e76a788cb5d86656) [2. b4249ed](https://github.com/zhanglab/psamm-model-collection/commit/b4249ed9d3a6a973e9b9c0195dfeaa4f6127e353) |
|[iFF708](sbml/iFF708)     | Allowed essential compounds in medium. | [f6a6f76](https://github.com/zhanglab/psamm-model-collection/commit/f6a6f76b09b521fa434e2ae09f0477094b32dde6) |
|[Multiple Models](sbml)   | Marked zeromass compounds in the following four models: iJN678, iRS1563, iRS1597, and iSyn669. | [405ee9d](https://github.com/zhanglab/psamm-model-collection/commit/405ee9dda1d4e6cc74e339c8e76a788cb5d86656) |
|[Multiple Models](sbml)   | Added biomass reaction definitions in the following seventeen models: AbyMBEL891, PpaMBEL1254, PpuMBEL1071, S_coelicolor, SpoMBEL1693, VvuMBEL943, iAC560, iAI549, iLC915, iMA945, iMM1415, iMO1056, iMR1_799, iPS189, iSR432, iSS884, and mus_musculus. | [b4249ed](https://github.com/zhanglab/psamm-model-collection/commit/b4249ed9d3a6a973e9b9c0195dfeaa4f6127e353) |

Model References
----------------

### Converted SBML Models

|Model|Reference|
|-----|---------|
|[AORYZAE_COBRA](sbml/AORYZAE_COBRA)     | Vongsangnak W, Olsen P, Hansen K, Krogsgaard S, Nielsen J (2008) _Improved annotation through genome-scale metabolic modeling of Aspergillus oryzae_. BMC Genomics 9: 245. <https://doi.org/10.1186/1471-2164-9-245>. |
|[AbyMBEL891](sbml/AbyMBEL891)        | Kim HU, Kim TY, Lee SY (2010) _Genome-scale metabolic network analysis and drug targeting of multi-drug resistant pathogen Acinetobacter baumannii AYE_. Mol Biosyst 6: 339–348. <https://doi.org/10.1039/b916446d>. |
|[AlgaGEM](sbml/AlgaGEM) | Gomes de Oliveira Dal’Molin, C., Quek, L.-E., Palfreyman, R. W., & Nielsen, L. K. (2011). AlgaGEM – a genome-scale metabolic reconstruction of algae based on the Chlamydomonas reinhardtii genome. BMC Genomics, 12(Suppl 4), S5. https://doi.org/10.1186/1471-2164-12-s4-s5 |
|[AraGEM](sbml/AraGEM)            | de Oliveira Dal’Molin C. G., Quek L. E., Palfreyman R. W., Brumbley S. M. & Nielsen L. K. _AraGEM, a genome-scale reconstruction of the primary metabolic network in Arabidopsis_. Plant Physiol. 152(2), 579–589 (2010).|
|[NmrFL413](sbml/NmrFL413) | Li, F., Xie, W., Yuan, Q., Luo, H., Li, P., Chen, T., Ma, H. (2018). Genome-scale metabolic model analysis indicates low energy production efficiency in marine ammonia-oxidizing archaea. AMB Express, 8(1). https://doi.org/10.1186/s13568-018-0635-y |
|[PpaMBEL1254](sbml/PpaMBEL1254)       | Sohn, Seung Bum, Alexandra B. Graf, Tae Yong Kim, Brigitte Gasser, Michael Maurer, Pau Ferrer, Diethard Mattanovich, and Sang Yup Lee. _Genome-scale Metabolic Model of Methylotrophic Yeast Pichia Pastoris and Its Use for in Silico Analysis of Heterologous Protein Production_. Biotechnology Journal, 2010, 705-15.|
|[PpuMBEL1071](sbml/PpuMBEL1071)       | Sohn, Seung Bum, Tae Yong Kim, Jong Myoung Park, and Sang Yup Lee. _In Silico Genome-scale Metabolic Analysis of Pseudomonas Putida KT2440 for Polyhydroxyalkanoate Synthesis, Degradation of Aromatics and Anaerobic Survival._ Biotechnology Journal, 2010, 739-50.|
|[RECON1](sbml/RECON1)            | Duarte, N. C., S. A. Becker, N. Jamshidi, I. Thiele, M. L. Mo, T. D. Vo, R. Srivas, and B. O. Palsson. _Global Reconstruction of the Human Metabolic Network Based on Genomic and Bibliomic Data_. Proceedings of the National Academy of Sciences, 2007, 1777-782. |
|[RECON2](sbml/recon2)            | Thiele, Ines, Neil Swainston, Ronan M T Fleming, Andreas Hoppe, Swagatika Sahoo, Maike K. Aurich, Hulda Haraldsdottir, Monica L. Mo, Ottar Rolfsson, Miranda D. Stobbe, Stefan G. Thorleifsson, Rasmus Agren, Christian Bölling, Sergio Bordel, Arvind K. Chavali, Paul Dobson, Warwick B. Dunn, Lukas Endler, David Hala, Michael Hucka, Duncan Hull, Daniel Jameson, Neema Jamshidi, Jon J. Jonsson, Nick Juty, Sarah Keating, Intawat Nookaew, Nicolas Le Novère, Naglis Malys, Alexander Mazein, Jason A. Papin, Nathan D. Price, Evgeni Selkov, Martin I. Sigurdsson, Evangelos Simeonidis, Nikolaus Sonnenschein, Kieran Smallbone, Anatoly Sorokin, Johannes H G M Van Beek, Dieter Weichart, Igor Goryanin, Jens Nielsen, Hans V. Westerhoff, Douglas B. Kell, Pedro Mendes, and Bernhard Ø Palsson. _A Community-driven Global Reconstruction of Human Metabolism_. Nat Biotechnol Nature Biotechnology 31.5 (2013): 419-25. |
|[Recon3D](sbml/Recon3D)  | King, Z. A., Lu, J., Dräger, A., Miller, P., Federowicz, S., Lerman, J. A., Ebrahim, A., Palsson, B. O., & Lewis, N. E. (2015). BiGG Models: A platform for integrating, standardizing and sharing genome-scale models. Nucleic Acids Research, 44(D1), D515–D522. https://doi.org/10.1093/nar/gkv1049 |
|[STM_v1.0](sbml/STM_v1.0)          | Thiele I, Hyduke DR, Steeb B, Fankam G, Allen DK, et al. (2011) _A community effort towards a knowledge-base and mathematical model of the human pathogen Salmonella Typhimurium LT2_. BMC Syst Biol 5: 8. <https://doi.org/10.1186/1752-0509-5-8>. |
|[S_coelicolor](sbml/S_coelicolor)      | Alam, Mohammad T., et al. "Metabolic modeling and analysis of the metabolic switch in Streptomyces coelicolor." BMC genomics 11.1 (2010): 202. <https://doi.org/10.1186/1471-2164-11-202>. |
|[S_coelicolor_fixed](sbml/S_coelicolor_fixed)| Alam, Mohammad T., et al. "Metabolic modeling and analysis of the metabolic switch in Streptomyces coelicolor." BMC genomics 11.1 (2010): 202. <https://doi.org/10.1186/1471-2164-11-202>. Fixed model from [m_model_collection](https://github.com/opencobra/m_model_collection/tree/2d3d0ab5115f4fca6b4a2cdb756d73586a510e5e). |
|[SpoMBEL1693](sbml/SpoMBEL1693)       | Sohn SB, Kim TY, Lee JH, Lee SY (2012) _Genome-scale metabolic model of the fission yeast Schizosaccharomyces pombe and the reconciliation of in silico/in vivo mutant growth_. <https://doi.org/10.1186/1752-0509-6-49>. |
|[VvuMBEL943](sbml/VvuMBEL943)        | Kim, H. U., S. Y. Kim, H. Jeong, T. Y. Kim, J. J. Kim, H. E. Choy, K. Y. Yi, J. H. Rhee, and S. Y. Lee. _Integrative Genome-scale Metabolic Analysis of Vibrio Vulnificus for Drug Targeting and Discovery_. Molecular Systems Biology 7.1 (2011): 460. Web.|
|[iAC560](sbml/iAC560)            | Chavali, Arvind K., Jeffrey D. Whittemore, James A. Eddy, Kyle T. Williams, and Jason A. Papin. _Systems Analysis of Metabolism in the Pathogenic Trypanosomatid Leishmania Major_. Mol Syst Biol Molecular Systems Biology 4 (2008): n. pag. Web.|
|[iAF1260](sbml/iAF1260)           | Feist AM, Henry CS, Reed JL, Krummenacker M, Joyce AR, et al. (2007) _A genome-scale metabolic reconstruction for Escherichia coli K-12 MG1655 that accounts for 1260 ORFs and thermodynamic information_. Mol Syst Biol 3: 121. <https://doi.org/10.1038/msb4100155>. |
|[iAF692](sbml/iAF692)            | Feist, Adam M., Johannes C M Scholten, Bernhard Ø Palsson, Fred J. Brockman, and Trey Ideker. _Modeling Methanogenesis with a Genome-scale Metabolic Reconstruction of Methanosarcina Barkeri_. Mol Syst Biol Molecular Systems Biology 2 (2006): n. pag. |
|[iAI549](sbml/iAI549)            | Ahsanul Islam M, Edwards EA, Mahadevan R (2010) _Characterizing the metabolism of Dehalococcoides with a constraint-based model_. PLoS Comput Biol 6. <https://doi.org/10.1371/journal.pcbi.1000887>. |
|[iBsu1103](sbml/iBsu1103)          | Henry CS, Zinner JF, Cohoon MP, Stevens RL. _iBsu1103: a new genome-scale metabolic model of Bacillus subtilis based on SEED annotations_. Genome Biol. 2009;10(6):R69. <https://doi.org/10.1186/gb-2009-10-6-r69>. |
|[iAK888](sbml/iAK888) | Klanchui, A., Dulsawat, S., Chaloemngam, K., Cheevadhanarak, S., Prommeenate, P., & Meechai, A. (2018). An Improved Genome-Scale Metabolic Model of Arthrospira platensis C1 (iAK888) and Its Application in Glycogen Overproduction. Metabolites, 8(4), 84. https://doi.org/10.3390/metabo8040084 |
|[iAp386B454](sbml/iAp386B454) | Pelicaen, R., Gonze, D., Teusink, B., De Vuyst, L., & Weckx, S. (2019). Genome-Scale Metabolic Reconstruction of Acetobacter pasteurianus 386B, a Candidate Functional Starter Culture for Cocoa Bean Fermentation. Frontiers in Microbiology, 10. https://doi.org/10.3389/fmicb.2019.02801 |
|[iCA1273](sbml/iCA1273)           | Archer CT, Kim JF, Jeong H, Park JH, Vickers CE, et al. (2011) _The genome sequence of E. coli W (ATCC 9637): comparative genome analysis and an improved genome-scale reconstruction of E. coli_. BMC Genomics 12: 9. <https://doi.org/10.1186/1471-2164-12-9>. |
|[iCB925](sbml/iCB925)            | Milne, Caroline B., et al. _Metabolic network reconstruction and genome-scale model of butanol-producing strain Clostridium beijerinckii NCIMB 8052_. BMC systems biology 5.1 (2011): 130. <https://doi.org/10.1186/1752-0509-5-130>. |
|[iCac802](sbml/iCac802)           | Dash, S., Mueller, T. J., Venkataramanan, K. P., Papoutsakis, E. T., & Maranas, C. D. (2014). _Capturing the response of Clostridium acetobutylicum to chemical stressors using a regulated genome-scale metabolic model_. Biotechnology for Biofuels, 7(1), 144.|
|[iCce806](sbml/iCce806)            | Vu TT, Stolyar SM, Pinchuk GE, Hill EA, Kucek LA, et al. (2012) _Genome-Scale Modeling of Light-Driven Reductant Partitioning and Carbon Fluxes in Diazotrophic Unicellular Cyanobacterium Cyanothece sp. ATCC 51142_. PLoS Comput Biol 8(4): e1002460. <https://doi.org/10.1371/journal.pcbi.1002460>. |
|[iCHOv1_final](sbml/iCHOv1_final) | Hefzi, H., Ang, K. S., Hanscho, M., Bordbar, A., Ruckerbauer, D., Lakshmanan, M., Orellana, C. A., Baycin-Hizal, D., Huang, Y., Ley, D., Martinez, V. S., Kyriakopoulos, S., Jiménez, N. E., Zielinski, D. C., Quek, L.-E., Wulff, T., Arnsdorf, J., Li, S., Lee, J. S., … Lewis, N. E. (2016). A Consensus Genome-scale Reconstruction of Chinese Hamster Ovary Cell Metabolism. Cell Systems, 3(5), 434–443.e8. https://doi.org/10.1016/j.cels.2016.10.020 |
|[iCZ946](sbml/iCZ946)  | Zuñiga, C., Levering, J., Antoniewicz, M. R., Guarnieri, M. T., Betenbaugh, M. J., & Zengler, K. (2017). Predicting Dynamic Metabolic Demands in the Photosynthetic Eukaryote Chlorella vulgaris. Plant Physiology, 176(1), 450–462. https://doi.org/10.1104/pp.17.00605 |
|[iFF708](sbml/iFF708)            | Forster, J. _Genome-Scale Reconstruction of the Saccharomyces Cerevisiae Metabolic Network_. Genome Research 13.2 (2003): 244-53. Web.|
|[iCZ843](sbml/iCZ843)| Zuñiga, C., Li, C.-T., Huelsman, T., Levering, J., Zielinski, D. C., McConnell, B. O., Long, C. P., Knoshaug, E. P., Guarnieri, M. T., Antoniewicz, M. R., Betenbaugh, M. J., & Zengler, K. (2016). Genome-Scale Metabolic Model for the Green Alga Chlorella vulgaris UTEX 395 Accurately Predicts Phenotypes under Autotrophic, Heterotrophic, and Mixotrophic Growth Conditions. Plant Physiology, 172(1), 589–602. https://doi.org/10.1104/pp.16.00593 |
|[iIB711](sbml/iIB711)            | Borodina, Irina, Preben Krabben, and Jens Nielsen. _Genome-scale analysis of Streptomyces coelicolor A3 (2) metabolism_. Genome research 15.6 (2005): 820-829. <https://doi.org/10.1101/gr.3364705>. |
|[iIT341](sbml/iIT341)            | Thiele, Ines, et al. _Expanded metabolic reconstruction of Helicobacter pylori (iIT341 GSM/GPR): an in silico genome-scale characterization of single-and double-deletion mutants_. Journal of bacteriology 187.16 (2005): 5818-5830. <https://doi.org/10.1128/JB.187.16.5818-5830.2005>. |
|[iJN678](sbml/iJN678)            | Nogales J, Gudmundsson S, Knight EM, Palsson BO, Thiele I (2012) _Detailing the optimality of photosynthesis in cyanobacteria through systems biology analysis_. Proc Natl Acad Sci U S A 109: 2678–2683. <https://doi.org/10.1073/pnas.1117907109>.|
|[iJN746](sbml/iJN746)            | Nogales J, Palsson BØ, Thiele I (2008) _A genome-scale metabolic reconstruction of Pseudomonas putida KT2440: iJN746 as a cell factory_. BMC Syst Biol 2: 79. <https://doi.org/10.1186/1752-0509-2-79>. |
|[iJO1366](sbml/iJO1366)           | Orth JD, Conrad TM, Na J, Lerman JA, Nam H, et al. (2011) _A comprehensive genome-scale reconstruction of Escherichia coli metabolism—2011_. Mol Syst Biol 7. <https://doi.org/10.1038/msb.2011.65>. |
|[iJP815](sbml/iJP815)            | Puchalka, J., M.A. Oberhardt, M. Godinho, A. Bielecka, D. Regenhardt, K.N. Timmis, J.A. Papin, and V.A.P. Martins dos Santos. 2008. _Genome-scale reconstruction and analysis of the Pseudomonas putida KT2440 metabolic network facilitates applications in biotechnology_. PLoS Computational Biology, 4(10):e1000210|
|[iJR904](sbml/iJR904)            | Reed JL, Vo TD, Schilling CH, Palsson BO. _An expanded genome-scale model of Escherichia coli K-12 (iJR904 GSM/GPR)_. Genome biology. 2003. January;4(9):R54 |
|[iRJ1321](sbml/iRJ1321)   | Shah, A. R., Ahmad, A., Srivastava, S., & Jaffar Ali, B. M. (2017). Reconstruction and analysis of a genome-scale metabolic model of Nannochloropsis gaditana. Algal Research, 26, 354–364. https://doi.org/10.1016/j.algal.2017.08.014  |
|[iKF1028](sbml/iKF1028)           | Fang K, Zhao H, Sun C, Lam CMC, Chang S, et al. (2011) _Exploring the metabolic network of the epidemic pathogen Burkholderia cenocepacia J2315 via genome-scale reconstruction_. BMC Syst Biol 5: 83. <https://doi.org/10.1186/1752-0509-5-83>. |
|[iLB1027_lipid](sbml/iLB1027_lipid) |  Levering, J., Broddrick, J., Dupont, C. L., Peers, G., Beeri, K., Mayers, J., Gallina, A. A., Allen, A. E., Palsson, B. O., & Zengler, K. (2016). Genome-Scale Model Reveals Metabolic Basis of Biomass Partitioning in a Model Diatom. PLOS ONE, 11(5), e0155038. https://doi.org/10.1371/journal.pone.0155038 |
|[iLC915](sbml/iLC915)            | Caspeta, Luis, et al. _Genome-scale metabolic reconstructions of Pichia stipitis and Pichia pastoris and in silico evaluation of their potentials_. BMC systems biology 6.1 (2012): 24. <https://doi.org/10.1186/1752-0509-6-24>. |
|[iMA871](sbml/iMA871)            | Andersen, Mikael Rørdam, Michael Lynge Nielsen, and Jens Nielsen. _Metabolic Model Integration of the Bibliome, Genome, Metabolome and Reactome of Aspergillus Niger_. Mol Syst Biol Molecular Systems Biology, 2008. |
|[iMA945](sbml/iMA945)            | AbuOun M, Suthers PF, Jones GI, Carter BR, Saunders MP, et al. (2009) _Genome scale reconstruction of a salmonella metabolic model comparison of similarity and differences with a commensal Escherichia coli strain_. J Biol Chem 284: 29480–29488. <https://doi.org/10.1074/jbc.M109.005868>. |
|[iMB745](sbml/iMB745)            | Benedict, M. N., M. C. Gonnerman, W. W. Metcalf, and N. D. Price. _Genome-Scale Metabolic Reconstruction and Hypothesis Testing in the Methanogenic Archaeon Methanosarcina Acetivorans C2A_. Journal of Bacteriology, 2011, 855-65. |
|[iMG746](sbml/iMG746) | Gonnerman, M. C., Benedict, M. N., Feist, A. M., Metcalf, W. W., & Price, N. D. (2013). Genomically and biochemically accurate metabolic reconstruction ofMethanosarcina barkeriFusaro, iMG746. Biotechnology Journal, 8(9), 1070–1079. https://doi.org/10.1002/biot.201200266 |
|[iMM1415](sbml/iMM1415)           | Sigurdsson MI, Jamshidi N, Steingrimsson E, Thiele I, Palsson BØ (2010) _A detailed genome-wide reconstruction of mouse metabolism based on human Recon 1_. BMC Syst Biol 4: 140. <https://doi.org/10.1186/1752-0509-4-140>. |
|[iMM904](sbml/iMM904)            | Mo ML, Palsson BO, Herrgård MJ (2009) _Connecting extracellular metabolomic measurements to intracellular flux states in yeast_. BMC Syst Biol 3: 37. <https://doi.org/10.1186/1752-0509-3-37>. |
|[iMO1056](sbml/iMO1056)           | Oberhardt, M.A., J. Puchalka, K.E. Fryer, V.A.P. Martins dos Santos, and J.A. Papin. 2008. _Genome-scale metabolic network analysis of the opportunistic pathogen Pseudomonas aeruginosa PAO1_. Journal of Bacteriology, 190(8). |
|[iMR1_799](sbml/iMR1_799)          | Ong WK, Vu TT, Lovendahl KN, Llull JM, Serres MH, et al. (2014) _Comparisons of Shewanella strains based on genome annotations, modeling, and experiments_. BMC Syst Biol 8: 1–11. |
|[iND750](sbml/iND750)            | Duarte NC, Herrgård MJ, Palsson BØ (2004) _Reconstruction and validation of Saccharomyces cerevisiae iND750, a fully compartmentalized genome-scale metabolic model_. Genome Res 14: 1298–1309. <https://doi.org/10.1101/gr.2250904>. |
|[iMZ1055](sbml/iMZ1055) | Zou, W., Zhou, M., Liu, L., & Chen, J. (2013). Reconstruction and analysis of the industrial strain Bacillus megaterium WSH002 genome-scale in silico metabolic model. Journal of Biotechnology, 164(4), 503–509. https://doi.org/10.1016/j.jbiotec.2013.01.019 |
|[iNJ661](sbml/iNJ661)            | Jamshidi, Neema, and Bernhard Ø. Palsson. "Investigating the metabolic capabilities of Mycobacterium tuberculosis H37Rv using the in silico strain iNJ661 and proposing alternative drug targets." BMC systems biology 1.1 (2007): 26. <https://doi.org/10.1186/1752-0509-1-26>. |
|[iNJ661v](sbml/iNJ661v)           | Fang X, Wallqvist A, Reifman J: _Development and analysis of an in vivo-compatible metabolic network of Mycobacterium tuberculosis_. BMC Syst Biol 2010, 4:160. |
|[iNJ661m](sbml/iNJ661m)           | Fang X, Wallqvist A, Reifman J: _Development and analysis of an in vivo-compatible metabolic network of Mycobacterium tuberculosis_. BMC Syst Biol 2010, 4:160. |
|[iNS934](sbml/iNS934)    | Loira, N., Mendoza, S., Paz Cortés, M., Rojas, N., Travisany, D., Genova, A. D., Gajardo, N., Ehrenfeld, N., & Maass, A. (2017). Reconstruction of the microalga Nannochloropsis salina genome-scale metabolic model with applications to lipid production. BMC Systems Biology, 11(1). https://doi.org/10.1186/s12918-017-0441-1 |
|[iOD907](sbml/iOD907)    | Dias, O., Pereira, R., Gombert, A. K., Ferreira, E. C., & Rocha, I. (2014). iOD907, the first genome-scale metabolic model for the milk yeastKluyveromyces lactis. Biotechnology Journal, 9(6), 776–790. https://doi.org/10.1002/biot.201300242 |
|[iPS189](sbml/iPS189)            | Suthers, Patrick F., Madhukar S. Dasika, Vinay Satish Kumar, Gennady Denisov, John I. Glass, and Costas D. Maranas. _A Genome-Scale Metabolic Reconstruction of Mycoplasma Genitalium, IPS189_. PLoS Comput Biol PLoS Computational Biology, 2009. |
|[iPS189_fixed](sbml/iPS189_fixed)      | Suthers, Patrick F., Madhukar S. Dasika, Vinay Satish Kumar, Gennady Denisov, John I. Glass, and Costas D. Maranas. _A Genome-Scale Metabolic Reconstruction of Mycoplasma Genitalium, IPS189_. PLoS Comput Biol PLoS Computational Biology, 2009. Fixed model from [m_model_collection](https://github.com/opencobra/m_model_collection/tree/2d3d0ab5115f4fca6b4a2cdb756d73586a510e5e). |
|[iRC1080](sbml/iRC1080)           | Chang RL, Ghamsari L, Manichaikul A, Hom EFY, Balaji S, et al. (2011) _Metabolic network reconstruction of Chlamydomonas offers insight into light-driven algal metabolism_. Mol Syst Biol 7: 518. <https://doi.org/10.1038/msb.2011.52>. |
|[iRS1563](sbml/iRS1563)           | Saha R, Suthers PF, Maranas CD (2011) _Zea mays iRS1563: A Comprehensive Genome-Scale Metabolic Reconstruction of Maize Metabolism_. PLoS ONE 6(7): e21784. <https://doi.org/10.1371/journal.pone.0021784>. |
|[iRS1597](sbml/iRS1597)           | Saha R, Suthers PF, Maranas CD (2011) _Zea mays iRS1563: A Comprehensive Genome-Scale Metabolic Reconstruction of Maize Metabolism_. PLoS ONE 6(7): e21784. <https://doi.org/10.1371/journal.pone.0021784>. |
|[iRsp1095](sbml/iRsp1095)          | Imam, Saheed, et al. _iRsp1095: a genome-scale reconstruction of the Rhodobacter sphaeroides metabolic network_. BMC systems biology 5.1 (2011): 116. <https://doi.org/10.1186/1752-0509-5-116>. |
|[iSB619](sbml/iSB619)            | Becker, S.A. and Pallson B.O. _Genome-scale reconstruction of the metabolic network in Staphylococcus auresus N315: an initial draft to the two-dimensional annotation_. BMC Microbiol., 5, 8, 2005. |
|[iSR432](sbml/iSR432)            | Roberts SB, Gowen CM, Brooks JP, Fong SS (2010) _Genome-scale metabolic analysis of Clostridium thermocellum for bioethanol production_. BMC Syst Biol 4: 31. <https://doi.org/10.1186/1752-0509-4-31>. |
|[iSS884](sbml/iSS884)            | Caspeta, Luis, et al. _Genome-scale metabolic reconstructions of Pichia stipitis and Pichia pastoris and in silico evaluation of their potentials_. BMC systems biology 6.1 (2012): 24. <https://doi.org/10.1186/1752-0509-6-24>. |
|[iSyn669](sbml/iSyn669)           | Montagud, Arnau, Emilio Navarro, Pedro Fernández De Córdoba, Javier F. Urchueguía, and Kiran Patil. _Reconstruction and Analysis of Genome-scale Metabolic Model of a Photosynthetic Bacterium_. BMC Systems Biology BMC Syst Biol 4.1 (2010): 156. |
|[iSyn731](sbml/iSyn731)           | Saha R, Verseput AT, Berla BM, Mueller TJ, Pakrasi HB, et al. (2012) _Reconstruction and Comparison of the Metabolic Potential of Cyanobacteria Cyanothece sp. ATCC 51142 and Synechocystis sp. PCC 6803_. PLoS One 7. <https://doi.org/10.1371/journal.pone.0048285>. |
|[iTH366](sbml/iTH366)            | Plata G, Hsiao T-L, Olszewski KL, Llinás M, Vitkup D (2010) _Reconstruction and flux-balance analysis of the Plasmodium falciparum metabolic network_. Mol Syst Biol 6: 408. <https://doi.org/10.1038/msb.2010.60>. |
|[iTZ479](sbml/iTZ479)            | Zhang, Y., I. Thiele, D. Weekes, Z. Li, L. Jaroszewski, K. Ginalski, A. M. Deacon, J. Wooley, S. A. Lesley, I. A. Wilson, B. Palsson, A. Osterman, and A. Godzik. _Three-Dimensional Structural View of the Central Metabolic Network of Thermotoga Maritima_. Science 325.5947 (2009): 1544-549|
|[iVS941](sbml/iVS941)            | Kumar, Vinay Satish, James G. Ferry, and Costas D. Maranas. _Metabolic Reconstruction of the Archaeon Methanogen Methanosarcina Acetivorans_. BMC Systems Biology BMC Syst Biol 5.1 (2011): 28 |
|[iVS941_fixed](sbml/iVS941_fixed)      | Kumar, Vinay Satish, James G. Ferry, and Costas D. Maranas. _Metabolic Reconstruction of the Archaeon Methanogen Methanosarcina Acetivorans_. BMC Systems Biology BMC Syst Biol 5.1 (2011): 28. Fixed model from [m_model_collection](https://github.com/opencobra/m_model_collection/tree/2d3d0ab5115f4fca6b4a2cdb756d73586a510e5e). |
|[iWZ583](sbml/iWZ583) | Zou, W., Xiong, X., Zhang, J., Zhang, K., Zhao, X., & Zhao, C. (2018). Reconstruction and analysis of a genome-scale metabolic model of Methylovorus sp. MP688, a high-level pyrroloquinolone quinone producer. Biosystems, 172, 37–42. https://doi.org/10.1016/j.biosystems.2018.07.009 |
|[iYL1228](sbml/iYL1228) | Liao, Yu-Chieh, et al. _An experimentally validated genome-scale metabolic reconstruction of Klebsiella pneumoniae MGH 78578, iYL1228_. Journal of bacteriology 193.7 (2011): 1710-1717. <https://doi.org/10.1128/JB.01218-10>. |
|[mus_musculus](sbml/mus_musculus) | Lake-ee Quek and Lars K. Nielsen (2008) _On the Reconstruction of the Mus musculus Genome-scale Metabolic Network Model_. Genome Informatics 2008: pp. 89-100. <https://doi.org/10.1142/9781848163324_0008>. |

### Converted Excel Models

|Model|Reference|
|-----|---------|
|[STM_v1.0](excel/STM_v1.0)           | Thiele I, Hyduke DR, Steeb B, Fankam G, Allen DK, et al. (2011) _A community effort towards a knowledge-base and mathematical model of the human pathogen Salmonella Typhimurium LT2_. BMC Syst Biol 5: 8. <https://doi.org/10.1186/1752-0509-5-8>. |
|[iCce806](excel/iCce806)            | Vu TT, Stolyar SM, Pinchuk GE, Hill EA, Kucek LA, et al. (2012) _Genome-Scale Modeling of Light-Driven Reductant Partitioning and Carbon Fluxes in Diazotrophic Unicellular Cyanobacterium Cyanothece sp. ATCC 51142_. PLoS Comput Biol 8(4): e1002460. <https://doi.org/10.1371/journal.pcbi.1002460>. |
|[iJO1366](excel/iJO1366)            | Orth JD, Conrad TM, Na J, Lerman JA, Nam H, et al. (2011) _A comprehensive genome-scale reconstruction of Escherichia coli metabolism—2011_. Mol Syst Biol 7. <https://doi.org/10.1038/msb.2011.65>. |
|[iMA945](excel/iMA945)             | AbuOun M, Suthers PF, Jones GI, Carter BR, Saunders MP, et al. (2009) _Genome scale reconstruction of a salmonella metabolic model comparison of similarity and differences with a commensal Escherichia coli strain_. J Biol Chem 284: 29480–29488. <https://doi.org/10.1074/jbc.M109.005868>. |
|[iMR1_799](excel/iMR1_799)           | Ong WK, Vu TT, Lovendahl KN, Llull JM, Serres MH, et al. (2014) _Comparisons of Shewanella strains based on genome annotations, modeling, and experiments_. BMC Syst Biol 8: 1–11. |
|[iNJ661](excel/iNJ661)             | Jamshidi, Neema, and Bernhard Ø Palsson. _Investigating the Metabolic Capabilities of Mycobacterium Tuberculosis H37Rv Using the in Silico Strain INJ661 and Proposing Alternative Drug Targets_. BMC Systems Biology BMC Syst Biol: 26. |
|[iNJ661v](excel/iNJ661v)            | Fang X, Wallqvist A, Reifman J. _Development and analysis of an in vivo-compatible metabolic network of Mycobacterium tuberculosis_. BMC Syst Biol 2010, 4:160.|
|[iNJ661m](excel/iNJ661m)            | Fang X, Wallqvist A, Reifman J. _Development and analysis of an in vivo-compatible metabolic network of Mycobacterium tuberculosis_. BMC Syst Biol 2010, 4:160.|
|[iSyn731](excel/iSyn731)            | Saha R, Verseput AT, Berla BM, Mueller TJ, Pakrasi HB, et al. (2012) _Reconstruction and Comparison of the Metabolic Potential of Cyanobacteria Cyanothece sp. ATCC 51142 and Synechocystis sp. PCC 6803_. PLoS One 7. <https://doi.org/10.1371/journal.pone.0048285>. |

### Converted MATLAB Models

|Model|Reference|
|-----|---------|
|[recon2.04](matlab/recon2.04)          | _Virtual Metabolic Human_. <https://vmh.uni.lu/>. Accessed October 9, 2015 from the page <https://vmh.uni.lu/#downloadview> using the link to <https://vmh.uni.lu/files/Recon2.v04.mat_.zip>. |
