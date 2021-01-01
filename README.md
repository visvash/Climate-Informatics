# Climate-Informatics 
Hello, I am <a href="https://www.linkedin.com/in/visvash-attri/">Visvash Attri</a>.  
I am working on a Machine Learning development focused on Geospatial Data. In this repo I am exploring and processing the data by demonstrating it through a Jupyter Notebook.  
Follow this Readme file for the entire walkthrough of the project.  
This project has been divided into four parts, or I should say "steps", those are mentioned below:  

### Steps  
- Procuring and Reading  
- Exploring and Visualizing  
- Preprocessing  
- Deep Learning  

# Procuring and Reading Geospatial Data
We are obtaining the data from the Copernicus Data Store <a href="https://cds.climate.copernicus.eu/cdsapp#!/home">(CDS)</a>.  
First and foremost, we need to install CDS API that helps to programmatically access to this data store.
#### Steps to install CDS API (Command Prompt)
- Create a CDS account by registering on the <a href="https://cds.climate.copernicus.eu/cdsapp#!/home">website</a>, and verify your email address provided.  
- Go to this <a href="https://cds.climate.copernicus.eu/api-how-to">page</a> and copy the 2 line code displayed in the black box in the "Install the CDS API key" section.
- In Command Prompt, write ``` type nul > .cdsapirc ``` and press Enter. (This will create a ```.cdsapirc``` file in 'C:\Users\username')
- Edit the ```.cdsapirc``` file with the help to a code editor. Paste the text copied in step 2, and save the file.  
- Install the CDS API client by running the following command in a Command Prompt window:  
  ```
  pip3 install cdsapi #for Python 3
  pip install cdsapi #for Python 2.7
  ```
  or try  
  ```
  pip install --user cdsapi #for Python 2.7
  pip3 install --user cdsapi #for Python 3
  ```
#### Steps to install CDS API (Anaconda Users)
- First four steps same as above method, open the Anaconda Prompt and run below two lines step by step  
  ```
  conda config --add channels conda-forge
  conda install cdsapi
  ```
