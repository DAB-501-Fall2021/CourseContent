# Week 4 - Data Visualization - Mapping vs. Setting

We will be using the dataset National Morbidity and Mortality Air Pollution Study (NMMAPS) to learn about ggobject and the difference between mapping and setting, as well as global and local mapping.  

First, load tidyverse package

Next, import the dataset from the Data Visualization folder using the readr package, available through tidyverse

```r
chicago <- read_csv(“https://raw.githubusercontent.com/DAB-501-Fall2021/CourseContent/main/Data%20Visualization/chicago-nmmaps.csv”)
```

Store current ggobject in variable g, including mappings

```r
g <- ggplot(chicago, aes(x=date, y=temp))
```

Extend ggobject g by adding other layers, including settings

```r
g + geom_point(colour = "firebrick", shape = "diamond", size = 2)
```

Now, extend the ggobject to other plot types.

Store new ggbject in variable p1, including labels

```r
p1 <- ggplot(chicago, aes(x = date, y = temp, color = season)) + 
           geom_point() + 
           labs(x = "Year", y = "Temperature (°F)")

```

Extend ggobject p1 by adding other geom_xxxx layers

```r
p1 + geom_rug()
```

# Week 3 - Data Visualization

We will be using the Pokemon dataset found from Kaggle at the link below to create visualizations.  The dataset contains both numerical and categorical data and it is available as a .csv file.  

https://www.kaggle.com/abcsds/pokemon?select=Pokemon.csv

Please go to the 'Data Visualization' folder to download the dataset and follow the instructions to contruct the visualizaitons.  

# Week 2 - Try Out Swirl

Head over to the Swirl folder listed above and try out the Swirl tutorials.  

Additional Swirl courses can be found at: http://swirlstats.com/scn/title.html


# Week 1 - Install R and RStudio

Welcome to DAB 501 Basic Statistics & Exploratory Data Analytics

We will be using GitHub to share data and R files to be used throughout the course.

Each main topic will have a folder where new content will be added weekly.  

Please feel free to refer back to the content to help with assignments and projects.
</br></br></br>

<b>First, install R:</b> https://cran.r-project.org/bin/windows/base/

Click on Download R 4.1.1 for Windows and wait for it to finish downloading. Run the executable file R-4.1.1-win.exe you just downloaded. Follow the installer instructions.

<b>Next, install RStudio:</b> https://www.rstudio.com/products/rstudio/download/#download

Under the Installers heading, click on RStudio 1.4.1717-Windows 10 and wait for it to finish downloading. Run the executable file RStudio-1.4.1717.exe you just downloaded. Follow the installer instructions.

