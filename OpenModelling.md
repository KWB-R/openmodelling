#Reproducibility in environmental modelling"
##Michael Rustler, Nicolas Caradot & Hauke Sonnenberg
###[Kompetenzzentrum Wasser Berlin gGmbH](http://kompetenz-wasser.de)

In environmental sciences numeric models play an important role supporting decision making. Usually, the modelling procedure (parameterisation, calibration, validation, scenario analysis) includes manual steps. 
For example, models are often calibrated by changing parameter values manually using a trial-and-error method (e.g. [Anibas et al. 2009](http://dx.doi.org/10.1002/hyp.7289)). 
This makes it challenging to document how the modelling software was used, which is a prerequisite for making the applied methodology transparent and thus the whole modelling process reproducible.

Automatation by means of programming can improve the modelling process. Once a methodology is implemented in the form of program code it is inherently documented. The code can be run repeatedly and will always produce the same results given the same inputs.

We used R as programming language to automate the modelling workflow.

Different models have been 'wrapped' by means of R packages ([Sonnenberg et al. 2014](http://dx.doi.org/10.13140/RG.2.1.2140.3683)): [Hantush (1967)](http://pubs.usgs.gov/sir/2010/5102/support/sir2010-5102.pdf) equation (groundwater mounding beneath an infiltration basin), [VS2DI](http://wwwbrr.cr.usgs.gov/projects/GW_Unsat/vs2di1.3/index.html) (groundwater flow, heat and solute transport), [WTAQ-2](http://water.usgs.gov/ogw/wtaq/) (well drawdown), [EPANET](http://www2.epa.gov/water-research/epanet) (pressurised pipe networks) and [Gompitz](http://doi.org/10.1080/15730620801939398) (sewer ageing). 

These models can now be configured and run from within the R environment. This allows to use R's excellent functions for retrieving and preparing input data (e.g. monitoring, geographical data) as well as analysing and plotting simulation results and generating reports.

Modelling is described in the form of version controlled R scripts so that its methodology becomes transparent and modifications (e.g. error fixing) trackable. This leads to reproducible results which should be the basis for smart decision making.   

#References

Anibas, C.; Fleckenstein,J.H.; Volze, N.; Buis, K.; Verhoeven, R.; Meire, P.; Batelaan, O. (2009): Transient or steady-state? Using vertical temperature profiles to quantify groundwater–surface water exchange, Hydrol. Process. 23, 2165 – 217, [http://dx.doi.org/10.1002/hyp.7289](http://dx.doi.org/10.1002/hyp.7289)

Hantush, M. S. (1967): Growth and decay of groundwater-mounds in response to uniform percolation, Water  Resources Research, March 1967, [http://doi.org/10.1029/WR003i001p00227](http://doi.org/10.1029/WR003i001p00227)

Sonnenberg, H.; Rustler, M.; Phillipon, V.; Caradot, N. & Matzinger, A. (2014): Wrap your model, Proceedings of the 11th International Conference on Hydroinformatics, New York City, USA, [http://dx.doi.org/10.13140/RG.2.1.2140.3683](http://dx.doi.org/10.13140/RG.2.1.2140.3683)

#R Package "kwb.hantush" 

For calculation of groundwater mounding beneath an infiltration basin:

- Stable: [http://cran.r-project.org/web/packages/kwb.hantush/index.html](http://cran.r-project.org/web/packages/kwb.hantush/index.html)

- Development & bug reporting: [https://github.com/KWB-R/kwb.hantush](https://github.com/KWB-R/kwb.hantush)

- Getting started: [http://kwb-r.github.io/kwb.hantush](http://kwb-r.github.io/kwb.hantush)





