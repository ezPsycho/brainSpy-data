# brainSpy-data
Transform your MNI coordinate to AAL Label and BA Label with brainSpy database.

## How to use the database

Install HDFS5 on your development environment, unzip `brainSpy.zip` and load `brainSpy.hdfs`.

The database contains following datasets: `aal.region`, `aal.distance`, `ba.region`, `ba.distance`, they are the region index and distance to nearest structure (the unit is mm).

To query the strcture information, just simply add 100, 150, 100 to the X, Y, and Z axes, and then use the new coordinates as an index to query the four data sets.

`aal.region` and `ba.region` only store the region index, to get region label, please checkout `aal_label.csv` and `ba_label.csv`.

## Data source

* The AAL template comes from [yunshiuan/label4MRI](https://github.com/yunshiuan/label4MRI);

* the BA template comes from [BioImage Suite](https://bioimagesuiteweb.github.io/webapp/).