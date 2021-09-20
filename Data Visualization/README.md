# Data Visualizations

First, click on the Pokemon.csv file above and inspect the data - what variables are included?  What types of data? Does it look complete?  Are there obvious errors? 

Next, click on 'Raw' to inspect the .csv file format.  Each line is a record where each record consists of more than one field separated by commas.  

Right click on the 'Raw' csv file and select 'Save As'.  Save the file as 'Pokemon.csv' to the Data folder inside the DAB501 project folder.  

Once the file is located in the Data folder, import the data in RStudio.  

In the console, type:

```{r}
Pokemon <-read.csv("~/Desktop/DAB501/Data/Pokemon.csv", header=TRUE) 
View(Pokemon)
```

Now inspect the data within RStudio.  Notice the headings are appropriately assigned considering header=TRUE in this case.  Make sure the tidyverse package is loaded in RStudio.

Create a plot using ggplot2 for Attack vs. Defense.  To begin, you may use the code below, then continue to improve the visualization by adding labels, colours, etc.

```{r}
ggplot(Pokemon, aes(x=Attack, y=Defense, colour=Type.1)) + geom_point()
```

Try making more visualizations using the Pokemon dataset.  

