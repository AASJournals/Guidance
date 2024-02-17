# Policy on Computational Notebooks and the AAS Journals
Chris Lintott and August Muench, February 2024

(This policy draws heavily on [Erdmann, C., Stall, S., Gentemann, C., Holdgraf, C., Fernandes, F. P. A., Gehlen, K. P., & Corvellec, M. (2021), _Guidance for AGU Authors - Jupyter Notebooks_, Zenodo](https://doi.org/10.5281/zenodo.4774440))

Much of the community served by the AAS Journals makes use of computational notebook tools (tools that combine text, code, and richer media in a single document), such as [Jupyter](https://jupyter.org/), to develop and share code used in research. Making these notebooks available to the reader of a paper may be extremely useful and is a significant contribution to reproducibility of the research contained within the publication. This short policy is intended to help those who wish to share their work this way, alongside the publication of a paper.

1. In preparing notebooks for a broad audience, we first recommend the advice in Rule, A. et al. (2021), [_Ten Simple Rules for Writing and Sharing Computational Analyses in Jupyter Notebooks_, PLOS Computational Biology](https://doi.org/10.1371/journal.pcbi.1007007)). In particular, we recommend giving thought to meaningful divisions between cells to help distinguish the different steps in any analysis and encourage plenty of explanatory text to help the reader understand what is happening. More detailed advice is available elsewhere, for example in this [Jupyter Notebooks and Tutorials guide](https://github.com/spacetelescope/style-guides/blob/master/guides/jupyter-notebooks.md) written by staff at STScI.

2. The AAS Journals, which aim to publish material that will be available for decades hence, do not presently accept submission of notebooks themselves as a part of a journal article. Notebooks should thus be uploaded to a public repository that can supply a Digital Object Identifier (DOI). One option is to create a GitHub repository that includes a suitable (open source) license and a [CITATION.cff](https://citation-file-format.github.io/#/what-is-a-citation-cff-file), and then using Zenodo to generate a DOI. (See [GitHub's Referencing and citing content Guide](https://guides.github.com/activities/citable-code/)). Alternative repositories that issue DOIs and have suitable archive policies may also be used; authors who are unsure should consult the AAS Data Editors (data-editors@aas.org) before submission.

Please note that it is extremely important to make clear explicitly in the notebook what dependencies are necessary for it to be used. A statement at the beginning of the notebook is often sufficient, but more advanced tools such as [conda-lock](https://pythonspeed.com/articles/conda-dependency-management/) to manage any dependencies may be useful.

**All data files required** to run the notebook should also be included in the DOI deposit. 

3. This DOI should be cited in the reference section of the paper and mentioned in the main text. An example statement might be: 

_The Jupyter Notebook to execute the analysis in this paper/to generate the figures in this paper is hosted at [e.g. Github] and is preserved on Zenodo at  [DOI]._

4. Making the notebook accessible to users with disabilities is very important. Using an [accessibility checklist](https://github.com/Iota-School/notebooks-for-all/blob/main/resources/event-hackathon/notebook-authoring-checklist.md) such as that created by the [Iota-School](https://iotaschool.com) in the “[Astronomy Notebooks for All](https://github.com/Iota-School/notebooks-for-all)” project may help in authoring more accessible notebooks.  

5. The first four steps describe the minimum requirements for including a Jupyter notebook in an AAS Journals paper. However, we strongly encourage authors to include a rendered (HTML, PDF, or ideally both) version of the notebook in their repository. Commands such as
```
jupyter nbconvert --to html --execute notebook.ipynb
jupyter nbconvert --to pdf --execute notebook.ipynb
```

Will usually produce useful files. A variety of hosted solutions may allow more advanced rendering, but even where these are used, simple HTML (and optionally PDF) versions should be included. 

Some examples of notebooks associated with published articles include:
 
> [https://doi.org/10.5281/zenodo.3945569](https://doi.org/10.5281/zenodo.3945569), accompanying Holwerda, B.W. et al., [2020, AJ, 160, 154](https://doi.org/10.3847/1538-3881/aba617)
> [https://doi.org/10.5281/zenodo.6226123](https://doi.org/10.5281/zenodo.6226123), accompanying Fullard, A.G. et al., [2022, ApJ, 930, 89](https://doi.org/10.3847/1538-4357/ac589e)
> [https://doi.org/10.5281/zenodo.7448504](https://doi.org/10.5281/zenodo.7448504), accompanying Mentuch Cooper, E. et al., [2023, ApJ, 943, 177](https://doi.org/10.3847/1538-4357/aca962) 
> [https://doi.org/10.5281/zenodo.7874710](https://doi.org/10.5281/zenodo.7874710), accompanying de los Reyes, M.A.C., et al. [2023, ApJ, 951, 52](https://doi.org/10.3847/1538-4357/acd189) 
