---
title: "Allocate storage positions to samples"
date: "2022-03-04"
---

  
If we want to track the storage position of samples, openBIS provides a graphical overview of lab storages. 

Lab storages need to be configured by a _lab manager_ or _group admin_, as explained here: [Configure Lab Storage](https://openbis.ch/index.php/docs/admin-documentation-openbis-20-10-3/customise-inventory-of-materials-and-samples/configure-lab-storage/)

  
This can be done in two ways:

1. add storage information on the sample form during (or after) sample registration
2. batch register storage positions for several samples  
      
    

##   
Register storage position for a single sample

1\. Navigate to the **Storage** section, at the bottom of the sample form. Click the **\+ New Storage Positions** above the table, as shown below:

![](https://openbis.ch/wp-content/uploads/2022/03/add-strorage-position.png)

  
2\. In the widget that opens, select the appropriate **Storage** from the dropdown menu. Storage must be configured by a lab manager or group admin as explained in [Configure Lab Storages](https://openbis.ch/index.php/docs/admin-documentation-20-10-3/customise-inventory-of-materials-and-samples/configure-lab-storage/)

![](https://openbis.ch/wp-content/uploads/2018/08/storage-selection-1024x202.png)

3\. Select the **position** in the storage (shelf and rack).

4\. If the sample is in a box, provide a **Box Name.**

5\. Select the **Box Size** form the list of configured sizes (the list can be configured by an _Instance Admin)_.

6\. Select the **Position** in the box.

7\. Click **Accept.**

![](https://openbis.ch/wp-content/uploads/2018/08/storage-assign-positions-1024x355.png)

### Add additional metadata to storage positions

  
By default, the storage only keeps track of locations. If the **Storage Position** has been configured by an _Instance admin_ to have additional metadata (e.g. freezing date), these can be added by clicking on the link in the storage table, as shown below. The link becomes available after saving the sample.

![](https://openbis.ch/wp-content/uploads/2022/03/storage-position-table-in-sample-1024x248.png)

The additional information can be entered in the **Storage Position** _Object_ form.

##   
Batch register storage positions

### XLS Batch Registration

With the new XLS batch registration, samples and their storage positions can be registered in one transaction using the XLS template file, as explained in [Batch register entries in a Collection](https://openbis.ch/index.php/docs/user-documentation-20-10-3/inventory-of-materials-and-methods/batch-register-entries-in-a-collection/).

### Batch Registration with TSV file

  
Storage positions are modelled in openBIS as children of other entries. To register the positions for several samples with the Batch Registration using the .tsv template, first the parent samples need to be registered in openBIS. In a second step, the positions are assigned.

To assign storage positions in batch mode follow the steps below:

> 1. Select **Storage positions** from the **Batch Registration** drop down menu.
> 2. Download the **template file**.
> 3. Remove the **identifier** column from the file (identifiers need to be automatically generated by openBIS).
> 4. Fill in the **parents** column. These are the identifiers of the samples for which we want to register the storage positions(/MATERIALS/PROJECT/OBJECT\_CODE).  
>     
> 5. Fill the remaining information about the storage positions.
> 6. Save the file and upload with the **Batch Registration**.

An example file can be found here: [SAMPLE-STORAGE\_POSITION-template.txt](https://wiki-bsse.ethz.ch/download/attachments/147412090/SAMPLE-STORAGE_POSITION-template.txt?version=1&modificationDate=1502441624183&api=v2)
