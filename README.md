# Ryan-Kennedy-Artifact-Senior-Project
Artifact repository for Ryan Kennedy's Senior Project at Allegheny College (this repo contains all of the code for the project)

# Ryan-Kennedy-Senior-Comp


## Introduction and Motivation-
**Summary of Project:** I have created an interactive dashboard (using Streamlit.io) that uses collected health data, specifically relating to food insecurity in Crawford County, PA, to produce interactive plots, graphs, and charts (using Plotly.express). I have also created an interactive map (using CARTO) that will reside on its own page on the dashboard. I intend for this dashboard to reside on the internet on its own app to be the most accessible to the public, especially for policymakers and food-insecure individuals to access it. The goal of the dashboard is to understand the variables affecting food insecurity, which parts of the county are being affected the most, who is being affected, where resources are located, how have food insecurity trends changed over time, possible methods that could resolve what leads to food insecurity, and to finally educate policymakers and food insecure individuals.


## Related Work-
[Beyond Food Deserts](https://www.brookings.edu/articles/beyond-food-deserts-america-needs-a-new-approach-to-mapping-food-insecurity)

[The Hidden Resilience of ‘Food ‘Desert’ Neighborhoods](https://civileats.com/2018/09/14/the-hidden-resilience-of-food-desert-neighborhoods/)

[Washington DC Food Deserts](https://jennyminich.carto.com/builder/d8836780-dbea-42f7-a5e6-0e3883fa570d/embed?state=%7B%22map%22%3A%7B%22ne%22%3A%5B38.75595740859807%2C-77.31113433837892%5D%2C%22sw%22%3A%5B38.974624157287955%2C-77.00317382812501%5D%2C%22center%22%3A%5B38.865374851611634%2C-77.15715408325197%5D%2C%22zoom%22%3A12%7D%7D)

[Access to Affordable and Nutritious Food: Measuring and Understanding Food Deserts and Their Consequences: Report to Congress](https://ageconsearch.umn.edu/record/292130/)

[Desert Wonderings: Reimagining Food Access Mapping](https://doi.org/10.1007/s10460-019-09914-5)

[Where Do Americans Usually Shop for Food and How Do They Travel To Get There? Initial Findings From the National Household Food Acquisition and Purchase Survey](https://www.ers.usda.gov/webdocs/publications/43953/eib138_errata.pdf?v=5900.1)

[Access to Affordable and Nutritious Food: Measuring and Understanding Food Deserts and Their Consequences: Report to Congress](https://ageconsearch.umn.edu/record/292130/)

[Understanding Accessibility to Snap-Accepting Food Store Locations: Disentangling the Roles of Transportation and Socioeconmoic Status](https://link.springer.com/article/10.1007/s12061-015-9138-2#citeas)

[Driving to save time or saving time to drive? The enduring appeal of the private car](https://www.sciencedirect.com/science/article/abs/pii/S0965856414000962?via%3Dihub)

[Comparing two distance measures in the spatial mapping of food deserts: The case of Petržalka, Slovakia](https://www.geonika.cz/EN/research/ENMGRClanky/2017_2_BILKOVA.pdf)

[Redefining the food desrt: combining GIS with direct observation to measure food access](https://link.springer.com/article/10.1007/s10460-014-9501-y)

[Identifying food insecurity in food sharing networks via machine learning](https://www.sciencedirect.com/science/article/pii/S0148296320306123?casa_token=p8HRyU2POioAAAAA:9hsJjvkdaPxDjB4c72Uchs1iJIJaY_KitSuOqcZcwb6Ez52z1ele2DOQ9zG8pPP0ExU49k9J4CA#b0205)


## Technical Details-
I use the programming language "Python" to create an interactive Streamlit dashboard. On this dashboard, there will be different pages which include: a Home Page, a General Comparative Analysis Page, a Food Insecurity Map Page, and a Contact Page. On the Home Page, I create text that describes what will be included in the rest of the dashboard, and the overall purpose of the dashboard. I also include text on each page to describe each dataset being used, each graph I have included, and the food insecurity map. To do this I use markdown built into Streamlit. To actually create each graph, I import the libraries "Pandas" and "Plotly", which I can then create data frames using my imported data and customize how I want each graph to be presented. The General Food Insecurity Comparative Analysis Graphs include a graph that compares Crawford County to every other county in Pennsylvania, and a graph that describes the past 8 years of Very Low Food Insecurity, Regular Food Insecurity, and the Food Environment Index specifically in Crawford County. On the Food Insecurity Map, I use the software CARTO and import various CSV, shapefile, and geojson files directly into CARTO, which the software can interpret and plot accordingly. Simultaneously, CARTO relies on the programming language SQL to create queries and manipulate each data table in order to overall determine which data from those files to plot on the map.  I also include a tool that allows each user to find the nearest food resources to them based on an inputted radius. This tool refers to the same data used in the map but also refers to imported libraries: ssl, geopy.geocoders, Nominatim, certifi, math, radians, sin, cos, sqrt, atan2. I finally included a Contact page which allows the user to directly send any feedback, give suggestions, or report an issue with my dashboard. This uses the software "FormSubmit". I also use some CSS to further format the input text boxes and submit button.


## Future Plans-
  I plan on adding a Predictive Analysis page to my dashboard. This will use logistic regression and neural network models to determine which variables in all of my data are the most significant in terms of making food insecurity worse every year, especially after the COVID-19 pandemic.
  
  I also plan on adding information about travel routes and travel options for food-insecure individuals. This may include plotting these on my CARTO map or displaying them in another fashion, easiest for policymakers and food-insecure individuals to understand. Furthermore, based on the transportation data, I could then create more interactive graphs.
  
  I plan on also adding data about the actual food being served in each food resource. This could include specific variables that affect the food environment index, food prices at each individual resource, or how healthy each resource is based on the type of food that is being offered.
  
  From including data on transportation and food nutrition, I could then add a tool that describes the overall accessibility score of each food resource. This could possibly help users determine which food resources to travel to the most.
  
  Finally, I plan on presenting the dashboard on its on app that is deployed on the internet. This would entice marketing that this dashboard exists, and spread the word to the correct audience (i.e. policymakers and food insecure individuals).

## How to Run Code (Locally)-
# Instructions to Run Streamlit Dashboard

So far, my Streamlit dashboard is only available locally on my own Mac machine, but it will be accessible to the public once I have finished my code and deployed my Streamlit app.

However, there are other ways to run the code on your own machine, for which I will provide below.

## Steps:

1. **Make Sure you have a source-code editor, such as Visual Studio Code, installed on your machine.**  
    1. Here is the link to download Visual Studio Code: [https://code.visualstudio.com/docs?dv=osx](url) . 
    2. Click on the download button in the upper right corner of the webpage.
    3. Drag the Visual Studio Code.app to the Applications folder prompted on the screen.
    4. Visual Studio Code should now be downloaded onto your machine!

2. **Install Python on your machine.**
    1. Navigate on your web browser to [python.org](url) and click on the "Downloads" tab. 
    2. Navigate and click on the type of machine you own (in my case it is macOS) and click on the "Download" link of the most recent release of Python (which currently is 3.12.0). This should start to download this version of Python to your machine when the installer is done downloading move on to the next step.
    3. Understand every prompt the installer puts on the screen (which includes the Introduction, Read Me, and License), and click on "Continue" to proceed forward after the prompts. You may be prompted to "Agree" to the terms of the software license agreement.
    4. Once you have gone through the  Introduction, Read Me, and License from the Installer, select the destination where you want the installer to install Python on your machine.
    5. After all previous steps are complete, Python should be successfully installed on your machine!

3. **Install the "PIP" package management system used to install and manage software packages/libraries written in Python.**
    1. Open your terminal.
    2. Navigate to the directory where you installed Python
    3. Run this command to download pip directly in that directory:
    ``` 
    curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
    ```
    4. Execute the downloaded file by running this command:
    ```
    python3 get-pip.py
    ```
    5. Walk through the installation process in your terminal
    6. PIP should now be installed on your machine!

4. **To run this Streamlit dashboard locally onto your computer, a directory for the code must be created first.**
    1. Open your terminal.
    2. navigate to where you desire to create the directory for the dashboard through using the cd , ls , or pwd commands.
    3. Once you have navigated to where you want the directory to exist, run this command:
    ```
    mkdir Interactive_Dashboard
    ```
    4. Naviagate into this directory using the command:
    ```
    cd Interactive_Dashboard
    ```
    5. Create other directories that will be used later. Make the first other directory using the command:
    ```
    mkdir pages
    ```
    6. Make the next directory using this command:
    ```
    mkdir style
    ```
    7. Make the final directory using this command:
    ```
    mkdir data
    ```

5. **Navigate into the Interactive_Dashboard directory**
    1. Run this command:
    ````
    cd Interactive_Dashboard
    ```

6. **Create Virtual Environment in Interactive_Dashboard Directory** 
    1. Run this command to create a virtual environment:
    ```
    python3 -m mvenv myvenv
    ```
        - Try this command if the previous one just mentioned does not work: 
        ```
        python -m venv ./venv
        ```

7. **Activate Newly Created Virtual Environment**
    1. Run this command to activate virtual environment:
    ```
    source myvenv/bin/activate
    ```
        - Try this command if the previous command just mentioned does not work: 
        ```
        source venv/Scripts/activate)
        ```
        - If using this alternate command, get out of this directory by typing: 
        ```
        cd ..
        ```
        - Fully get out of the next directory by typing the command: 
        ```
        cd ..
        ``` 
        - Finally, ensure you are now still in the "Interactive_Dashboard" directory.

8. **Install all necessary packages and libraries using PIP**
    1. Run these commands one at a time in your terminal to install all packages refered to in the code:
    ```
    pip install streamlit
    pip install plotly_express==0.4.0
    pip install pandas
    pip install ssl
    pip install geopy
    pip install certifi
    ```

9. **Open VS Code and Install the code . Shell Command**
    1. Open Visual Studio Code from your Applications folder on your machine.
    2. Once opened, Open the Command Palette (Cmd+Shift+P)
    3. Type: code .  in the search box
    4. The code . should now be installed!

10. **Run the "code ." Command in Terminal to Open New Window in VS Code Specifically for the Interactive_Dashboard Directory**
    1. Run this command:
    ``` 
    code .
    ```

11. **Create Python File inside the Interactive_Dashboard Directory**
    1. Run this command to create a new Python file in the Interactive_Dashboard directory, which should also appear in the newly opened Visual Studio Code window:
    ```
    code 1_🏠_Home Page.py
    ```

12. **Download the Data and Other Files From my GitHub Repository, Into the Interactive_Dashboard Directory**
    1. In my GitHub Repository, navigate into my folder titled "dashboard". 
    2. Click on the file titled "1_🏠_Home Page.py".
    3. Copy all code in this code by selecting all code and pressing:
    Cmd+c.
    4. Paste this code into the previously created "1_🏠_Home Page.py" python file in your own "Interactive_Dashboard" directory by pressing:
    Cmd+v.
    5. In my GitHub Repository, navigate into my folder titled "pages".
    6. Click on and download each one of these .py files by selecting one at a time and clicking the download button on the top right of the screen.
    7. Drag or insert these files into your directory titled "pages" within the "Interactive_Dashboard" directory on your machine. Make sure to keep these files only within the "pages" directory.
    8. In my GitHub Repository, navigate into my folder titled "style".
    9. Click and download the file titled "style.css" in the way previously described.
    10. Drag or insert this file into your directory titled "style" within the "Interactive_Dashboard" directory on your machine. Make sure to keep this file only within the "style" directory.
    11. Finally, in my GitHub Repository, navigate into my folder titled "data".
    12. Click on and download each one of these .csv files in the way previously described.
    13. Drag or insert these files into your directory titled "data" within the "Interactive_Dashboard" directory on your machine. Make sure to keep these files only within the "data" directory.

13. **Change the Path of Each Dataframe in Python Files**
    1. In the previously downloaded Python files "2_📈_General_Comparative_Analysis.py" and "3_🗺️_Food_Insecurity_Map.py", CSV files are being imported for data usage, which the Pandas library uses as input to create a dataframe for each CSV file. In order for the code to run correctly, you must replace the path of those files where they are stored on your machine instead of mine.
    2. The code in the General_Comparative_Analysis.py file to import the CSV files and make the dataframes will look like:
    ```py
    df = pd.read_csv("/Users/ryankennedy/Desktop/Interactive_Dashboard/Crawford_County_General_Food_Insecurity_Data.csv")

    dataframe = pd.read_csv("/Users/ryankennedy/Desktop/Interactive_Dashboard/General_Food_Insecurity_Data_Two.csv") 
    ```
    The code in the Food_Insecurity_Map.py file to import the CSV files and make the dataframes will look like:
    ```py
    food_resources1_df = pd.read_csv('/Users/ryankennedy/Desktop/Food_Insecurity_Data/Food_Insecurity_Data_CSV_Files/Radius_Formula_CSV_Files/Crawford_County_Food_Resource_Locations_Radius.csv')

    food_resources2_df = pd.read_csv('/Users/ryankennedy/Desktop/Food_Insecurity_Data/Food_Insecurity_Data_CSV_Files/Radius_Formula_CSV_Files/Supermarkets_and_Grocery_Stores_Located_within_Crawford_County_PA_Radius.csv')

    food_resources3_df = pd.read_csv('/Users/ryankennedy/Desktop/Food_Insecurity_Data/Food_Insecurity_Data_CSV_Files/Radius_Formula_CSV_Files/Fast_Food_Establishments_Radius.csv')
    ```
    3. The names of each CSV file will be at the end of the code with the suffix ".csv".
    4. An easy way to find the path of each of these files is to open a new terminal window, and drag and dtop each file into the window. This will automatically give the exact path to where each file resides on your machine.
    4. Once you have the path to each file, copy and paste the path where my path is in each line of code that corresponds with that CSV file. You want to paste your path in the parameters within the ' ' marks after each pandas method "pd.read_csv".
    5. Once each path is replaced with your own, all of the code should work smoothly! 

14. **Run a Streamlit server that uses the Downloaded Files**
    1. Run this command to create and run a Streamlit server on the internet using the newly created Python file:
    ```
    streamlit run 1_🏠_Home Page.py
    ```
    2. Once this command is run, your default web browser should appear with a blank Streamlit interface, as no code in the Python file has been applied yet.
    3. Your terminal should now have given you two URL links, one for the Local URL of the Streamlit app, and one for the Network URL of the Streamlit app. Save both of these links somewhere safe.
    4. On the Streamlit app, click on the "Always Re-run" button in the top right corner of the page. This will allow the Streamlit app to always be updated when there are any changes to the code, and those changes are saved.
    5. Now, in the Streamlit server and dashboard should update with the newly inputted code in the Dashboard.py file!  If it does not update at first, try reloading the page.
    6. Do NOT close the terminal window.

15. **To Safely Close Streamlit app in Terminal**
    1. To safely close the Streamlit app in the first terminal opened, push these buttons on your keyboard at the same time:
    Crl+c
    2. Streamlit in your terminal should have given you a message that says something similar to "app stops running (yay!)".
 
 16. **Open Streamlit App After Closing It**
    1. To open the streamlit app again, run this command in your terminal once you have navigated into the Interactive_Dashboard directory:
    ```
    streamlit run Dashboard.py
    ```
    2. To only open the Streamlit app on your web browser, refer to the local URL you copied and stored in a safe place earlier. Clicking on this link should bring you to the Streamlit app!


All steps have now been completed to successfully run the Code in my GitHub Repository for my Prototype!
