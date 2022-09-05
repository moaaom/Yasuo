## FOR BIOL3207 WORKSHOP #6
BY Yusheng & Ruijia

---

## ABOUT

The repo main introduces how to use Git and Github, and calculate mean activity for each treatment for each species and visualise it.

---

## DATA CONTENT

The ".rmd" file is the main coding file, which can do some certain data process.

The "data" floder includes original data from [Clark et al., 2020](https://doi.org/10.1038/s41586-019-1903-y), which will be used as a data resource.

The "output" floder includes outcomes of these codes, in which the "data" and " figures" floders include results of processed tables and figures. The file is not tracked by Github.

The "pics" floder includes six ".png" files, which will involve in the process as background figures of each fish species.

The "README" file includes some instructions.

The ".html" file is the output markdown of ".rmd" file.

The ".Rproj" file help you set the work direction.

The ".gitignore" file includes direction that not be tracked.

The ".Rhistory" file includes history of  R of the process.

---

## HOW TO USE

1. Put data into the "data" file. The detailed meta-data for each column are as follows:

| Column Name | Description|
| - | - |
| loc | Location, and year, where the data were collected. AIMS = Australian Institute of Marine Science; LIRS = Lizard Island Research Station|
| species | Species name: acantho = Acanthochromis; Ambon = Pomacentrus amboinensis; Chromis = Chromis atripectoralis; Humbug = Dascyllus aruanus; Lemon = Pomacentrus moluccensis|
| treatment | Elevated CO2 [CO2] (850-1,050 µatm) or control [Control] (400 - 450 µatm) groups|
| animal_id | Fish identity|
| sl | Standard length of the fish in mm|
| size | Size grouping of the fish, separated at 15 mm standard length into ‘big’ or ‘small’|
| activity | Number of seconds the fish was active per minute, averaged across the duration of the trial|
| comment | Comment with notes on the origin of the data|

If you use other data, please DO NOT change the file name "OA_activitydat_20190302_BIOL3207.csv".

2. Put figures of the six fish species (names shown in each figure name) into the "pics" file. If you use other data, please DO NOT change the file names of the figures.

3. Knit the ".rmd" file.

---

## READ RESULTS

1. The file in direction "./output/data" is a processed data removed missing value and irrelevant columns from original data. The detailed meta-data for each column are as follows:

| Column Name | Description |
| - | - |
| species | Species name: acantho = Acanthochromis; Ambon = Pomacentrus amboinensis; Chromis = Chromis atripectoralis; Humbug = Dascyllus aruanus; Lemon = Pomacentrus moluccensis| 
| treatment | Elevated CO2 [CO2] (850-1,050 µatm) or control [Control] (400 - 450 µatm) groups|
| sample_size | The sample size of each kind of fish|
| mean_sl | The mean of standard length of the fish in mm of each kind of fish|
| se_sl | The standard error of standard length of the fish in mm of each kind of fish|
| mean_activity | The mean of number of seconds the fish was active per minute of each kind of fish|
| se_activity | The standard error of number of seconds the fish was active per minute of each kind of fish|

2. The figures in direction "./output/figures" are about mean activity for each treatment for each species, with or without backgrounds relying on figures in the "pics" floder.

3. The ".html" file shows results of each step of the process.
