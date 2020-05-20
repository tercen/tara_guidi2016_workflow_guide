# Data analysis workflow of TARA Oceans data using Tercen

This document describeds a walkthrough example of data analysis and visualisation using Tercen.

We will analyse data from the TARA Oceans project, from this publication.

Our goal is to:

* Look at environmental variables and how plankton are distributed

* Second goal

## Create a Tercen project

* Click on New project

* Assign a team

* Give a name and description to this project

## Loading data into Tercen

**1. Download the data onto your computer**

We will use data from Guidi et al. (2016). It can be found here. Click on Download.

**2. Go back to Tercen and load the data**

Now that we have the data on our computer, we can import it into Tercen.

* Go to the project we named TARA Oceans

![](./img/loaddata1.png)

![](./img/loaddata2.png)

![](./img/loaddata3.png)

![](./img/loaddata4.png)

![](./img/loaddata5.png)

## Data preprocessing


![](./img/workflow1.png)

![](./img/workflow2.png)

![](./img/workflow3.png)

![](./img/workflow4.png)

![](./img/workflow5.png)

## Making a heatmap

**1. Adding a data step**

![](./img/datastep1.png)

![](./img/datastep2.png)

**2. Making the heatmap projection**

<iframe src="https://drive.google.com/file/d/1jPIbcZGZFpHAnPLrlawR6S489_vEYc3H/preview" width="640" height="480"></iframe>

### Clustering and dendrogram

**3. Improving the heatmap**

This heatmap look nice, but what if it would look much better if we could order rows and columns and add dendrograms!

Tercen includes a **heatmap operator** to make such a representation.

On the left, click to add an operator:

Pick `shiny_heatmap_operator`

![](./img/operator1.png)


Tercen includes two types of operators: shiny and regular ones. Shiny operators are mostly designed to visualise data in a given step rather than perform a specific computation.

When the operator is loaded, you can see a tab appeared on the left: **Operator view**. Let's click on it.

The operator view appeared, as well as our heatmap with a dendrogram!

![](./img/operator2.png)

## Making a world map

Coming soon.