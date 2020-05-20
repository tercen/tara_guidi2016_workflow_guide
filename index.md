# Analysing TARA Oceans carbon export data using Tercen

This document describes a walkthrough example of data analysis and visualisation using **Tercen**. We will analyse data from the TARA Oceans project, coming from this publication: [Guidi et al. (2016)]().

Our goal is to look at **how eukaryotic plankton lineages are associated to environmental parameters** such as **carbon export**. To do so, we will:

* create a new project in Tercen

* upload the dataset containing the correlation of different lineages to environmental parameters

* create a heatmap representing this correlation

### Creating a Tercen project

* Click on New project

<center><img src="./img/project1.png" alt="" width="600"/></center>

* Assign a team

* Give a name and description to this project

<center><img src="./img/project2.png" alt="" width="400"/></center>

### Loading data into Tercen

**1. Download the data onto your computer**

We will use data from Guidi et al. (2016). It can be found here. Click on Download.

**2. Go back to Tercen and load the data**

Now that we have the data on our computer, we can import it into Tercen.

* Go to the project we named TARA Oceans

<center><img src="./img/loaddata1.png" alt="" width="600"/></center>

<center><img src="./img/loaddata2.png" alt="" width="400"/></center>

<center><img src="./img/loaddata3.png" alt="" width="400"/></center>

<center><img src="./img/loaddata4.png" alt="" width="400"/></center>


### Creating a workflow

<center><img src="./img/loaddata5.png" alt="" width="600"/></center>

<center><img src="./img/workflow1.png" alt="" width="600"/></center>

<center><img src="./img/workflow2.png" alt="" width="400"/></center>

<center><img src="./img/workflow3.png" alt="" width="400"/></center>

### Making a heatmap

**1. Adding a data step to the workflow**

<center><img src="./img/workflow4.png" alt="" width="600"/></center>

<center><img src="./img/workflow5.png" alt="" width="400"/></center>

**2. Making the heatmap projection**

Double click on the newly created data step. 

Drag and drop elements to make the heatmap projection.

<center><img src="./img/datastep1.png" alt="" width="600"/></center>

<center><img src="./img/datastep2.png" alt="" width="600"/></center>

Here is a video of this important step:

<center><iframe src="https://drive.google.com/file/d/1jPIbcZGZFpHAnPLrlawR6S489_vEYc3H/preview" width="600" height="400"></iframe></center>

**3. Improving the heatmap by ordering rows and columns and adding dendrograms**

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