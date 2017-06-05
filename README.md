# anisotropy_prediction

## Summary:
Perform statistical analysis and data conditioning of well log data, use predictive modeling to estimate vertical resistivity and electrical anisotropy using commonly available well log parameters. Follow-on from [work presented at EAGE 2016](http://www.rocksolidimages.com/pdf/2016_EAGE_Predicting_Electrical_Anisotropy.pdf).  

## Background:
Electrical resistivity within the earth is an important property for the detection of oil and gas, making it valuable to measure remotely, in two or three dimensions. A challenge arose - traditionally, data collected at the site of a drilled well included only resistivity measurements taken perpendicular to the well path, but assuming that the resistivity is the same in all directions (electrical isotropy) led to poorly parameterized remote surveys and incorrect analysis of the resulting data. Recently, well measurements of resistivity in both a horizontal (perpendicular to well path) and vertical (parallel to well path) direction have been made, which allow for better survey design and calibration of the remotely-measured data, but these data are rare.

This project began as part of a multi-year research consortium project investigating electrical anisotropy. The initial work was done using a geoscience analytics package. I have since reworked the project using open source tools in preparation for publication. 

Using data from one well location which includes both horizontal and vertical resistivity measurements, I performed exploratory data analysis to identify relationships between standard well log measurements and vertical resistivity, condition the data appropriately, split the data into training and test sets, and used regression modeling to statistically predict vertical resistivity and electrical anisotropy. I validated these predictions using the reserved test dataset, with the remotely measured data I had analyzed previously, and with data from an additional well located a few hundred km away that became available after the initial project ended.

As the input data are covered by an NDA, and the results cannot be fully shared prior to publication, the Jupyter notebook associated with this work is private at this time, but may be made available, in whole or part, at a later date.

## Tools used:
- [Jupyter notebooks](http://jupyter.org/install.html)
- [pandas](http://pandas.pydata.org)
- [numpy](http://www.numpy.org)
- [scikit-learn](http://scikit-learn.org)
- [matplotlib](http://matplotlib.org)
- [seaborn](http://seaborn.pydata.org)
- [lasio](https://github.com/kinverarity1/lasio)
