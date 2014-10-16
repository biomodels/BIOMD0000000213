# BIOMD0000000213: Folate2004

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000213.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000213.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000213 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This is an SBML version of the folate cycle model model from:  
**A mathematical model of the folate cycle: new insights into folate homeostasis.**   
_Nijhout HF, Reed MC, Budu P, Ulrich CM_ J. Biol. Chem.,2004, **279**
(53),55008-16  
pubmedID: [15496403](http://www.ncbi.nlm.nih.gov/pubmed/15496403)  
Abstract:  
A mathematical model is developed for the folate cycle based on standard
biochemical kinetics. We use the model to provide new insights into several
different mechanisms of folate homeostasis. The model reproduces the known
pool sizes of folate substrates and the fluxes through each of the loops of
the folate cycle and has the qualitative behavior observed in a variety of
experimental studies. Vitamin B(12) deficiency, modeled as a reduction in the
V(max) of the methionine synthase reaction, results in a secondary folate
deficiency via the accumulation of folate as 5-methyltetrahydrofolate (the
"methyl trap"). One form of homeostasis is revealed by the fact that a
100-fold up-regulation of thymidylate synthase and dihydrofolate reductase
(known to occur at the G(1)/S transition) dramatically increases pyrimidine
production without affecting the other reactions of the folate cycle. The
model also predicts that an almost total inhibition of dihydrofolate reductase
is required to significantly inhibit the thymidylate synthase reaction,
consistent with experimental and clinical studies on the effects of
methotrexate. Sensitivity to variation in enzymatic parameters tends to be
local in the cycle and inversely proportional to the number of reactions that
interconvert two folate substrates. Another form of homeostasis is a
consequence of the nonenzymatic binding of folate substrates to folate
enzymes. Without folate binding, the velocities of the reactions decrease
approximately linearly as total folate is decreased. In the presence of folate
binding and allosteric inhibition, the velocities show a remarkable constancy
as total folate is decreased.  
This model was encoded by Michal Galdzicki from a MatLab file send to him by
Prof. Michael Reed. There some differences in this model compared to the one
described in the article, possible due to typos in the publication:  
1) reaction NE (THF + H2CO <=> 5,10-CH2-THF) in the article has H2C=O as a
reactant and is mentioned to display pseudo first order mass action kinetics,
while in the matlab file formic acid, also used in reaction FTS, is included
in the rate law for the forward reaction.  
2) the reaction MS is modeled after Reed et al. 2004, which is not explicitly
mentioned in the article, although Kd and the parameters from Reed et al. 2004
are given.  
3) in the kinetic law of the SHTM reaction (THF + Ser <=> 5,10-CH2-THF + Gly),
there are separate values given for Km,Gly and Km,5,10-CH2-THF in the article.
in the matlab file and the SBML model Km,Ser and Km,THF are used instead of
Km,Gly and Km,5,10-CH2-THF for the backwards reaction.

  

To the extent possible under law, all copyright and related or neighbouring
rights to this encoded model have been dedicated to the public domain
worldwide. Please refer to [CC0 Public Domain
Dedication](http://creativecommons.org/publicdomain/zero/1.0/) for more
information.

In summary, you are entitled to use this encoded model in absolutely any
manner you deem suitable, verbatim, or with modification, alone or embedded it
in a larger context, redistribute it, commercially or not, in a restricted way
or not.

  

To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


