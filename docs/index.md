# Analysing TARA Oceans carbon export data using Tercen

This document describes a walkthrough example of data analysis and visualisation using **Tercen**. We will analyse data from the TARA Oceans project, coming from this publication: [Guidi et al. (2016)]().

Our goal is to look at **how eukaryotic plankton lineages are associated to environmental parameters** such as **carbon export**. To do so, we will:

* create a new project in Tercen

* upload the dataset containing the correlation of different lineages to environmental parameters

* create a heatmap representing this correlation

### Creating a Tercen project

First, we will create a Tercen project for our analyses.

* **Start Tercen** and **log in**

* Click on **New project**

<center><img src="./img/project1.png" alt="" width="600"/></center>

* **Assign the team** of your choice to the project

* Give a **name** and **description** to this project, then click on **OK**

<center><img src="./img/project2.png" alt="" width="400"/></center>

* Your project is now created !

### Loading data into Tercen



**1. Download the data onto your computer**

We will use data from Guidi et al. (2016), more specifically the Supplementary Table 5. You can download data here: [LINK]. In this tutorial, we will just use the `SI5_eukaryotic_lineages.tsv` file.

**2. Go back to Tercen and load the data**

Now that we have the data on our computer, we can import it into Tercen.

* Go to the newly created project

* Click on **New data set**

<center><img src="./img/loaddata1.png" alt="" width="600"/></center>

* **Upload** the `SI5_eukaryotic_lineages.tsv` file (**1**)

* Give a **name** to the data set (**2**)

* Click on **Next** (**3**)

<center><img src="./img/loaddata2.png" alt="" width="400"/></center>

* Check that the data set has been loaded properly and click on **Next**

<center><img src="./img/loaddata3.png" alt="" width="400"/></center>

* HARD PART TO EXPLAIN and click on **OK**

<center><img src="./img/loaddata4.png" alt="" width="400"/></center>

### Creating a workflow

Now that we have created our dataset, we will **create a workflow** to analyse and visualise it.

* Click on **New workflow**

* Give a **name** to your workflow

<center><img src="./img/loaddata5.png" alt="" width="600"/></center>

* Your workflow appears now in your project. **Click on it**

* Your are now on the workflow environment that is empty. We will now **add the data set** we uploaded before. **Right click anywhere in the blank area** and click on **Add**.

<center><img src="./img/workflow1.png" alt="" width="600"/></center>

* **Select Table** and click on **OK**.

<center><img src="./img/workflow2.png" alt="" width="400"/></center>

* **Select the data set** and click on **OK**.

<center><img src="./img/workflow3.png" alt="" width="400"/></center>

* Now the data set is ready to be used !

### Making a heatmap

To analyse our data we need to:

**1. Add a data step to the workflow**

<center><img src="./img/workflow4.png" alt="" width="600"/></center>

<center><img src="./img/workflow5.png" alt="" width="400"/></center>

**2. Make the heatmap projection**

Double click on the newly created data step. 

Drag and drop elements to make the heatmap projection.

<center><img src="./img/datastep1.png" alt="" width="600"/></center>

<center><img src="./img/datastep2.png" alt="" width="600"/></center>

Here is a video of this important step:

<center><iframe src="https://drive.google.com/file/d/1jPIbcZGZFpHAnPLrlawR6S489_vEYc3H/preview" width="600" height="400"></iframe></center>

**3. Improve the heatmap by ordering rows and columns and adding dendrograms**

This heatmap look nice, but what if it would look much better if we could order rows and columns and add dendrograms!

Tercen includes a **heatmap operator** to make such a representation.

On the left, click to add an operator:

Pick `shiny_heatmap_operator`

<center><img src="./img/operator1.png" alt="" width="600"/></center>


Tercen includes two types of operators: shiny and regular ones. Shiny operators are mostly designed to visualise data in a given step rather than perform a specific computation.

When the operator is loaded, you can see a tab appeared on the left: **Operator view**. Let's click on it.

The operator view appeared, as well as our heatmap with a dendrogram!

<center><img src="./img/operator2.png" alt="" width="600"/></center>

*Et voilà!*