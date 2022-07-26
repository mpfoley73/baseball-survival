This project is a statistical analysis of the association between longevity (life expectancy) and fame in Major League baseball. It is inspired by Redelmeier and Singh's [survival in Oscar winners study](http://fisher.utstat.toronto.edu/reid/sta442f/2009/aawards.pdf) which found that winning an Academy Award was associated with 3.9 years of additional life expectancy. In this setting, fame conferred by induction into the baseball Hall of Fame replaces the Academy Award.

## What the project does

* **Evaluate data sources**. There are at least two data sources that can support this project. [Retrosheet](https://www.retrosheet.org/biofile.htm) publishes a single text file of players that is easy to work with and comprehensive, but somewhat limited in the number of attributes. [Lahman's Baseball Database](https://www.seanlahman.com/baseball-archive/statistics/) is an entire data model. It has an associated [R package](https://github.com/cdalzell/Lahman) and it was also used in [a similar study](http://www.med.mcgill.ca/epidemiology/hanley/bios601/CandHchapter06/baseball_players.pdf) by Abel and Kruger.
* **Review Literature**. The two studies referenced above lay the foundation that this study will build upon. In addition, Redelmeier and Singh recently published [an update to their Academy study](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0266563) in PLoS ONE.
  * **abel_kruger_2005** ([html](https://mpfoley73.github.io/baseball-survival//abel_kruger_2005.html), [Rmd](../src/abel_kruger_2005.Rmd)). Reproduction of Abel & Kruger 2005 study (incomplete - I'm struggling with the data setup.)
  * **saint_onge_2008** ([html](https://mpfoley73.github.io/baseball-survival//saint_onge_2008.html), [Rmd](../src/saint_onge_2008.Rmd)). Review of *Major League Baseball Players' Life Expectancies* ([2008](#SaintOnge2008)). Partially reproduces the 2008 analysis using the **Lahman** data, re-fits their discrete-time logistic regression models with data updated through the 2021 season, and fits an alternative Cox proportional hazards model.
* **Groundwork**. The Abel and Kruger study is so similar to this study, both is subject and data source, that reproducing their results will be a good exercise in working with the data.

## Why the project is useful

I'm not a professional in age studies, so it is unlikely that this project makes a meaningful contribution to the literature on survival. However, it will be an end-to-end analysis with accessible data and code that analysts may reference and learn from for survival studies. It includes Kaplan Meier survival curve exploration and Cox proportional hazards regression analysis.

## Who maintains and contributes to the project

I worked on this project independently. Project is under development.

## References

[Baseball with R](https://baseballwithr.wordpress.com/) blog.

Ernest L. Abel & Michael L. Kruger (2005) The Longevity of Baseball Hall of Famers Compared to Other Players, Death Studies, 29:10, 959-963, DOI: [10.1080/07481180500299493](https://doi.org/10.1080/07481180500299493). [PDF](http://www.med.mcgill.ca/epidemiology/hanley/bios601/CandHchapter06/baseball_players.pdf).

[Lahman](https://github.com/cdalzell/Lahman). Sean Lahman's R Package.

Lemez S, Baker J. Do Elite Athletes Live Longer? A Systematic Review of Mortality and Longevity in Elite Athletes. Sports Med Open. 2015;1(1):16. doi:10.1186/s40798-015-0024-x. [PDF](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4534511/).

Redelmeier, D. A., & Singh, S. M. (2001). Survival in Academy Award–winning actors and actresses. Annals of Internal Medicine, 134(10), 955-962. [PDF](http://fisher.utstat.toronto.edu/reid/sta442f/2009/aawards.pdf).

Redelmeier DA, Singh SM (2022) Long-term mortality of academy award winning actors and actresses. PLoS ONE 17(4): e0266563. [https://doi.org/10.1371/journal.pone.0266563](https://doi.org/10.1371/journal.pone.0266563)

[Retrosheet](https://www.retrosheet.org/biofile.htm).

<a id="SaintOnge2008"></a>Saint Onge JM, Rogers RG, Krueger PM. Major League Baseball Players' Life Expectancies. Soc Sci Q. 2008;89(3):817-830. doi:10.1111/j.1540-6237.2008.00562.x. [HTML](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2743321/).

[Sean Lahman's Baseball Database](https://www.seanlahman.com/baseball-archive/statistics/).

Smith G. The Baseball Hall of Fame is not the kiss of death. Death Stud. 2011 Nov-Dec;35(10):949-55. doi: 10.1080/07481187.2011.553337. PMID: 24501860. [PDF](https://www.researchgate.net/profile/Gary-Smith-8/publication/260118629_The_Baseball_Hall_of_Fame_Is_Not_the_Kiss_of_Death/links/5485b3620cf24356db610de9/The-Baseball-Hall-of-Fame-Is-Not-the-Kiss-of-Death.pdf).

Sylvestre, Marie-Pierre & Huszti, Ella & Hanley, James. (2006). Do Oscar Winners Live Longer than Less Successful Peers? A Reanalysis of the Evidence. Annals of internal medicine. 145. 361-3; discussion 392. 10.7326/0003-4819-145-5-200609050-00009. [PDF](https://www.researchgate.net/publication/6836472_Do_Oscar_Winners_Live_Longer_than_Less_Successful_Peers_A_Reanalysis_of_the_Evidence).

[Survival Analysis](https://bookdown.org/mpfoley1973/supervised-ml/survival-analysis.html). My supervised machine learning notes on survival analysis.

