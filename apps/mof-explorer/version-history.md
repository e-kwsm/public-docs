---
description: >-
  Changes made to the QMOF Database:
  https://doi.org/10.6084/m9.figshare.13147324
---

# Version History

## Changelog

* [v14](https://figshare.com/articles/dataset/QMOF\_Database/13147324/14): New single-point calculations at the HLE17, HSE06\* (i.e. 10% HF ex.), and HSE06 (25% HF ex.) levels of theory. 12/09/21.
* [v13](https://figshare.com/articles/dataset/QMOF\_Database/13147324/13): Locked-in version to match the PBE files [uploaded to NOMAD](https://nomad-lab.eu/prod/rae/gui/dataset/id/O-FUAo0mThSUeXg70cMN3Q?results=entries). 09/15/21.
* [v12](https://figshare.com/articles/dataset/QMOF\_Database/13147324/12): Several MOFs taken from the [Genomic MOF Database](https://figshare.com/s/ec378d7315581e48f1e4) with over/underbonded atoms were removed, as the original authors of the Genomic MOF Database uploaded a fairly large fraction of structures with missing H atoms. Supplemental results from new non-self-consistent (NSCF) calculations with a higher k-point density are now provided (note: this was reverted in v13, as it was discovered that LMAXMIX was [not set high enough](https://github.com/materialsproject/pymatgen/commit/932d9da8c19d30040990bd273550e996c7d7519d), effecting the NSCF results for a subset of structures). Removed raw VASP files from Figshare to instead host them on [NOMAD](https://nomad-lab.eu/prod/rae/gui/dataset/id/O-FUAo0mThSUeXg70cMN3Q). Gave each MOF a unique hash-based identifier, which will match the identifiers on the forthcoming Materials Project MOF Explorer app. 09/14/21.
* [v11](https://figshare.com/articles/dataset/QMOF\_Database/13147324/11): Same changes as in v12, but the bandgaps.csv file was not made backwards-compatible here. 09/13/21.
* [v10](https://figshare.com/articles/dataset/QMOF\_Database/13147324/10): Removed irrelevant data from the JSON, reducing the filesize. 09/01/21.
* [v9](https://figshare.com/articles/dataset/QMOF\_Database/13147324/9): Added \~3000 new DFT-optimized MOFs from the CoRE MOF Database (based on the clean subset identified by [Chen and Manz](https://doi.org/10.1039/D0RA02498H)), the [Genomic MOF Database](https://figshare.com/s/ec378d7315581e48f1e4), and the CSD MOF Subset. Deprecated 13 structures. Added spacegroup info. Added "synthesized?" flag. Added missing PLDs and LCDs. Fixed 186 structures that had EDIFF = 1e-4 instead of EDIFF = 1e-6 in the INCAR. Removed structures that were duplicates according to Pymatgen's StructureMatcher to avoid confusion. The user no longer needs to run the StructureMatcher as a result. 09/01/21.
* [v8](https://figshare.com/articles/dataset/QMOF\_Database/13147324/8): Added 1243 new DFT-optimized MOFs. 623 were taken from the [Boyd & Woo dataset](https://doi.org/10.24435/materialscloud:2018.0016/v3), 485 were taken directly from the [2019 CoRE MOF FSR Database](https://doi.org/10.5281/zenodo.3677685), 92 were Cu triangle MOFs taken from [ToBaCCo](https://pubs.acs.org/doi/abs/10.1021/acs.cgd.7b00848), and 44 were Hf MOFs obtained by exchanging the Zr metals of ToBaCCo MOFs by [Anderson and coworkers](https://osf.io/7dgvy/). For the CoRE MOFs, only those found in [this pre-curated list](https://doi.org/10.1021/acs.jctc.0c01229) were included to maximize structural fidelity. For the hypothetical MOFs, some new ones were introduced using the Boyd & Woo structures as a starting point (e.g. by exchanging metal cations). 3 MOFs were deprecated. Added MOFids, DOIs, spin-dependent CBM/VBM, and initial CIFs for the hypothetical MOFs. 07/12/21.
* [v7](https://figshare.com/articles/dataset/QMOF\_Database/13147324/7): Deprecated 12 MOFs. Added more properties to JSON file and made it easier to parse. 06/08/21.
* [v6](https://figshare.com/articles/dataset/QMOF\_Database/13147324/6): Added 2620 DFT-optimized MOFs. 1217 were taken from the CSD using the usual protocol. 1188 were hypothetical MOFs obtained from the [Boyd & Woo dataset](https://doi.org/10.24435/materialscloud:2018.0016/v3). 148 were hypothetical MOF-74 and MOF-5 analogues obtained from Haranczyk's [nanoporousmaterials.org](http://nanoporousmaterials.org/databases/). 48 were hypothetical Zr MOFs made with [ToBaCCo](https://github.com/tobacco-mofs/tobacco\_3.0) and obtained from [Anderson and coworkers](https://osf.io/7dgvy/). 19 were experimental pyrene MOFs from [Smit and coworkers](https://doi.org/10.24435/materialscloud:z5-ct). The maximum number of atoms per unit cell was raised to 500. 5/7/2021.
* [v5](https://figshare.com/articles/dataset/QMOF\_Database/13147324/5): Release corresponding to the published [_Matter_ paper](https://www.cell.com/matter/fulltext/S2590-2385\(21\)00070-9). No changes to the database compared to v3. Fixes a bug in `get_subset_data.py` that did not correctly write out the updated `.json` file. 2/12/21.
* [v4](https://figshare.com/articles/dataset/QMOF\_Database/13147324/4): Includes a few minor typo fixes and better `.xlsx` reader. 1/12/21.
* [v3](https://figshare.com/articles/dataset/QMOF\_Database/13147324/3): Added CM5 partial charges for every structure and 3000+ Bader charges (and spin densities). Patched some minor bugfixes with the unrelaxed properties for a few MOF structures, deprecated a few structures, and flagged more duplicates. Continued restructuring of main QMOF database for increased useability. 12/23/20.
* [v2](https://figshare.com/articles/dataset/QMOF\_Database/13147324/2): \~1500 new structures with pore-limiting diameter greater than 2.4 Å, computed using Zeo++ prior to structure relaxation, were added to the QMOF database along with their DFT-computed properties. The cap on the maximum number of atoms per primitive cell was raised from 150 to 300. 12/05/20.
* [v1](https://figshare.com/articles/dataset/QMOF\_Database/13147324/1): Initial release corresponding to the QMOF database [pre-print](https://dx.doi.org/10.26434/chemrxiv.13147616). 10/28/20.