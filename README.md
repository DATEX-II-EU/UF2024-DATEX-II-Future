# UF2024-DATEX-II-Future

Exploring the future of DATEX II

Workshop leader: Jörg Freudenstein
The workshop is done together with Ian, Paal and Jonas

We will present planned and envisaged methodologies and features of DATEX II,

and the participants are engaged to bring in their own ideas for the future development. On a practical technical example, we will show some planned possibilities of the DATEX II version 4 methodology like Entities and APIs. Filtering requests will be served by a test server, so that participants can re-enact at home.

# Simple demo server access (without using Jupyter Notebook)

Just run this query in the browser. No installation necessary. You can play around with the parameters.

https://v4futureapi.azurewebsites.net/GetAccidentsByRadius?accidentType=accident&radius=3&latitude=53.476531&longitude=-2.328261

<i>Demo limitation: The parameter accidentType is not mandatory, but in order to get results, it must be present as shown above. There is no filtering on accident types, i.e. all kind of accident types (here in the demo: 2 different types) are returned.</i>

# Client-side code generation with Java (using Jupyter Notebook)

In the Jupyter Notebook, there are instruction to create the necessary code with OpenAPI generator and some python code fragments to request accident information from the demo server (filtered by coordinates and radius). The resulting accidents are displayed on a map.

Intructions:
* Install Jupyter Notebook: https://jupyter.org/install
* Copy the two files from the repository into the <code>Jupyter</code> folder of your jupiter-installation:<br> The Jupyter Notebook file (.ipynb) and the YAML-File
  <br>
  It is not necessary to copy any files from the <code>supporting</code> folder.
* Download this OpenAPI Generator file into the same folder:<br> https://repo1.maven.org/maven2/org/openapitools/openapi-generator-cli/7.9.0/openapi-generator-cli-7.9.0.jar<br>
  (Note: You need a Java installation to run this later)
* And of course you need Python to be installed (e.g. https://www.python.org/downloads/)
* Now run from command line: <code>jupyter notebook</code>. It will open jupyter in your browser.
* Browse into the <code>Jupyter</code> folder and open the <code>DATEX_II_v4-Demo.ipynb</code> notebook.
* Follow the further steps in the notebook.

### DATEX Schema Generation Tool, demo version v4

This link is also used during the steps in the notebook:
https://datexfutureexample.azurewebsites.net/
