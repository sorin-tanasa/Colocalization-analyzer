# Colocalization analyzer
 Simple data visualization shiny app for colocalization

A Python pipeline was developed to analyze the colocalization of two markers in specific foci when cells are submitted to a putative cancer drug that induces cell death. The foci form prior to the death onset and may serve as a clue into the mechanism of action of that drug. Visualizations in Python are typically done in the Mathplotlib library, with less aesthetic possibilities. This R Shiny  Colocalization analyzer application was developed to give the more customizable and aesthetic output.

The Colocalization analyzer can be run in an Rstudio GUI or off a server with the link provided. The online app is hosted on a virtual Linux server from AWS and can be accessed at the following address:
http://3.75.183.31:3838/data_analyzer/

The application takes a single input (input.csv) file and outputs a single figure (plot.png). It contains:
1. Upload csv data file - Browse button, which can be used to find the location of the file
2. X Axis title and Y Axis title respetively, which are optional and can be left empty, or filled in to give the names of the X and Y axes
3. Input height (px) and Input weight (px) - required fields to set the height and weight of the figure. They become activated initially by pressing the "Update plot" button, then automatically when changed. 
4. Update plot button, which initializes the figure in the Shinyapp and later must be called to update height and width whenever the user changes those parameters
5. Download plot button - in the offline version it can be used to set a download location and save simultaneously, while in the server version it automatically downloads the plot.png file to the default Download folder.

The tpyical use is exemplified in the folowowing way:

1. Initialization - the window will look like this when initialized:
 <br />
<img width="960" alt="initial window" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/e886e002-57d5-464e-8f69-f326b5d50388">
<br />
<br />
<br />
2. File selection:
<br />
<img width="959" alt="file uploaded" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/4c96a549-ee0d-45cf-a267-c9b7812de1cd">
<br />
<br />
<br />
3. Detail update - plot height and width must be supplied as integer (natural) numbers. Titles for the X and Y columns are optional:
<br />
<img width="955" alt="all fields filled in" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/80dad226-0a31-4c0a-992d-d82c6785b23e">
<br />
4. Generating the plot - pressing the Update plot button generates the figure:
<br />
<img width="958" alt="all fields filled and graph generated" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/8ac68469-f8ac-4583-b927-3e3f5004daa2">
<br />
The figure itself is visualised bellow the buttons, taking up a large window space, and can be fully visualized by scrolling the window down:
<br />
<img width="942" alt="graph generated bellow the buttons" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/2524582f-13de-476c-b491-86f59c08cbf0">
<br />
Larger resolutions will not fit well in the GUI but can be also generated as outputs:
<img width="959" alt="all fields filled in for larger image" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/e0474a21-54f1-4781-8461-57b7fb3119d6">

<img width="959" alt="all fields filled in for larger image" src="https://github.com/neomaster117/Colocalization-analyzer/assets/47111504/3a718418-ea1b-45ac-b83b-9de79b8d5a91">



The actual images may look different and the user should customize the figure by also checking the output itself. Bellow we can see two outputs created with different settings:


