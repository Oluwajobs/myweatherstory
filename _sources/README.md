# myweatherstory
This Jupyter Book provides a sample lesson activity on how to run the WRF model on a raspberry pi. It is intended to be used in conjunction with NCAR's Pi-WRF project. The idea is to provide a location to contain information content related to Pi-WRF. This could include teaching modules that target atmospheric science and concepts relevant for further understanding the computational components of Pi-WRF.

Contributions from outside of NCAR are encouraged. The maintainer of the project is Agbeli Ameko: agbeli@ucar.edu

To make changes to any activity in this notebook, first clone the repo using ```git clone https://github.com/Oluwajobs/myweatherstory/```. Next, make your edits and commit the changes using: ```git add . && git commit -m "<commit message>"```. Afterwards, you will need to rebuild the notebook and publish it using the following commands.

```
# build book after changes have been made to the repo
# from the parent directory that contains the myweatherstory/ directory
jupyter-book build myweatherstory/

# This will rebuild the html, incorporating any changes to the files. 
ghp-import -npf myweatherstory/_build/html
```
The website can be found at: https://oluwajobs.github.io/myweatherstory/
