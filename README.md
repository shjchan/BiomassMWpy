# BiomassMWpy
Python functions for determining the chemical formulae and molecular weights of macromolecules in genome-scale metabolic models.  
Please see the following paper for more details:  
Siu H. J. Chan, Jingyi Cai, Lin Wang, Margaret N. Simons-Senftle, Costas D. Maranas (2017) Standardizing biomass reactions and ensuring complete mass balance in genome-scale metabolic models, *Bioinformatics*, 33(22), 3603–3609.
**[Link](https://doi.org/10.1093/bioinformatics/btx453)**  

Require **[Cobrapy](https://github.com/opencobra/cobrapy)**(>=0.15.1). See the help files for documentation.  

Main object: `biomassmw`.  
It is initialized with a cobra model. Use the following two methods to calculate chemical formulae or the range for biomass MW:  
- `.compute_met_form`: Compute the chemical formulas of the unknown metabolites given the formulas for a set of known metabolites using a set of reactions.  
- `.compute_met_range`: Compute the minimum and maximum possible MW of the target metabolite.
