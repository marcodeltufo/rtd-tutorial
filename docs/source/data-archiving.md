---
title: "Data archiving"
date: "2022-02-23"
---

 

# Dataset archiving

 

openBIS supports archiving of datasets to Strongbox ([https://www.strongboxdata.com/](https://www.strongboxdata.com/)) as described in [Datasets Archiving](https://unlimited.ethz.ch/display/openBISDoc2010/Archiving+Datasets)

 

This needs to be set up and configured by a _system admin_.

 

To trigger archiving manually from the ELN, navigate to a dataset and use the _Request or disallow archiving_ button, as shown below.

 

![](https://openbis.ch/wp-content/uploads/2021/06/archiving-button.png)

 

 

 

Please note that the strongbox has a minimum size requirement of **10GB**. If a single dataset is below this threshold it will be queued for archiving and it will be archived only when additional datasets in the same _Space/Project/Experiment_ are selected for archiving and the minimum size is reached. All datasets are bundled together and archived together. This implies that if unarchiving is requested for one dataset in a bundle, all other datasets will also be unarchived.

 

## Dataset archiving helper tool

 

If you wish to archive multiple datasets, you can use the **Archiving Helper** tool under **Utilities** in the main menu. You can search for datasets and select multiple ones to be archived, by clicking the **Request Archiving** button on the top of the page.

 

![](https://openbis.ch/wp-content/uploads/2022/02/archiving-helper-1024x529.png)

 

# Dataset unarchiving

 

Once the dataset is archived on tapes, the button on the dataset page changes to **Unarchive**, as shown below. Datasets can be unarchived by using this button.

 

![](https://openbis.ch/wp-content/uploads/2021/06/Unarchive.png)

 

 

## Dataset unarchiving helper tool

 

To unarchive several datasets it is possible to use the **Unarchiving Helper** tool, under **Utilities** in the main menu, as shown below. You can search for datasets and select multiple ones to be unarchived, using the **Unarchive** button on tope of the page.

 

![](https://openbis.ch/wp-content/uploads/2021/06/unarchive-helper-tool.png)
