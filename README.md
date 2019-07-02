# Demo PyQt 5
DemoPyQT 5

# Description of files 

Main.py is the python file that contains all the code for the demo

2017.csv is the initial datasets, it is raw data that is used in the first graphic of the application.

final_happiness_dataset.csv is the processed dataset that is used in most of the graphs and in the ML algorithms

analisis.png and enter.png are icons that are used in the menu items in the application

all the files need to be located in the same directory

# Technical considerations

1. Main is PYQ5 application, thus, pyq5 needs to be installed in the computer in order to execute this app.

2. The application also uses graphviz-2.38, be user to have it installed in the computer

    The directory that uses this application for graphviz-2.38 is:
    
       'C:\\Program Files (x86)\\graphviz-2.38\\release\\bin'
       
    If you have it installed in another path, change this path at the top of the Main.py file.

3. The applicaiton also uses a *font_size_window = 'font-size:15px'* at the top of the Main.py file, if you wich , it can be changed, just be sure to use the correct sintax for your stylesheet font size.


# Description of the application 

The purpose of the application is to present a basic EDA analysis of the processed dataset and two dashboards with the results of the algoritms. The algorithms used are Random Forest Classifier and Decision Tree. These two models can be run separately but the complement each other since both gives information that is relevant for making recommendadtions.

The structure of the application is as follows 

1. File
  * Exit : it quits  the application
2. EDA Analysis
  * Initial Assesment : This option presents a frequency histogram. Groups the number o countries by happiness score.
  * Happiness Final : This option presents a plot graphic that shows the relation of each feature in the final datasets with the happiness score. A line can be draw optionaly to represent the tendency of the data.
  * Correlation Plot : This option presents a correlation plot for all the features in the dataset. The features can be add o deleted from the plot. Each time that a modification is made the button **Create Plot** should be pressed.
3. ML Models
  * Decision Tree Algorithm
  * Random Forest Classifier
