This project is a statistical analysis of the association between longevity (life expectancy) and fame in Major League baseball. It is inspired by Redelmeier and Singh's [survival in Oscar winners study](http://fisher.utstat.toronto.edu/reid/sta442f/2009/aawards.pdf) which found that winning an Academy Award was associated with 3.9 years of additional life expectancy. In this setting, fame conferred by induction into the baseball Hall of Fame replaces the Academy Award.

Project Plan

* **Evaluate data sources**. There are at least two data sources that can support this project. [Retrosheet](https://www.retrosheet.org/biofile.htm) publishes a single text file of players that is easy to work with and comprehensive, but somewhat limited in the number of attributes. [Lahman's Baseball Database](https://www.seanlahman.com/baseball-archive/statistics/) is an entire data model. It has an associated [R package](https://github.com/cdalzell/Lahman) and it was also used in [a similar study](http://www.med.mcgill.ca/epidemiology/hanley/bios601/CandHchapter06/baseball_players.pdf) by Abel and Kruger.
* **Review Literature**. The two studies referenced above lay the foundation that this study will build upon. In addition, Redelmeier and Singh recently published [an update to their Academy study](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0266563) in PLoS ONE.
* **Groundwork**. The Abel and Kruger study is so similar to this study, both is subject and data source, that reproducing their results will be a good exercise in working with the data.

## What the project does

TBD. This project is a survival analysis. 

## Why the project is useful

I'm not a professional in age studies, so it is unlikely that this project makes a meaningful contribution to the literature on survival. However, it will be an end-to-end analysis with accessible data and code that analysts may reference and learn from for survival studies. It includes Kaplan Meier survival curve exploration and Cox proportional hazards regression analysis.

## Who maintains and contributes to the project

I worked on this project independently. Project is under development.

## References

Ernest L. Abel & Michael L. Kruger (2005) The Longevity of Baseball Hall of Famers Compared to Other Players, Death Studies, 29:10, 959-963, DOI: [10.1080/07481180500299493](https://doi.org/10.1080/07481180500299493). [PDF](http://www.med.mcgill.ca/epidemiology/hanley/bios601/CandHchapter06/baseball_players.pdf).

Redelmeier, D. A., & Singh, S. M. (2001). Survival in Academy Award–winning actors and actresses. Annals of Internal Medicine, 134(10), 955-962. [PDF](http://fisher.utstat.toronto.edu/reid/sta442f/2009/aawards.pdf).

Redelmeier DA, Singh SM (2022) Long-term mortality of academy award winning actors and actresses. PLoS ONE 17(4): e0266563. [https://doi.org/10.1371/journal.pone.0266563](https://doi.org/10.1371/journal.pone.0266563)

[Retrosheet](https://www.retrosheet.org/biofile.htm).

[Sean Lahman's Baseball Database](https://www.seanlahman.com/baseball-archive/statistics/).

[Lahman](https://github.com/cdalzell/Lahman). Sean Lahman's R Package.

[Baseball with R](https://baseballwithr.wordpress.com/) blog.

