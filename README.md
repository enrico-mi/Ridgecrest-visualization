## Ridgecrest webapp

This repository contains all the code necessary to locally run the interactive web app that complements the submitted manuscript *Coseismic damage of the 2019 Ridgecrest earthquake consistent with Mohr-Coulomb failure* (Milanese and Cattania, 2024). The webapp is also accessible at <http://www.enricomilanese.com/Ridgecrest>.

### Downloading the data

The webapp both performs real-time analyses and visualizations and loads pre-analysed datasets and figures. The latter is due to a combination of how the project evolved and of analyses that are too heavy to be performed in real-time.

The datasets are accessible at *[this Harvard Dataverse repository](https://doi.org/10.7910/DVN/HCFAEO)*.

If you believe you should have access to those data but for some reason cannot, reach out to me at enricomi@mit.edu.

Once you unzip the archive, the data are already in their own folders (`geojson` and `SRw`), and you just need to move those folder at the root of this git repository (i.e. where `index.html` is).

### Launching the webapp

To launch a local server to host the webapp you can just follow the steps below. I'm assuming you have python3.

1. Navigate to the root-directory of this project, where the file `index.html` is

2. Execute the following in the command line

		python3 -m http.server 8000
   
3. Open your browser and visit <http://localhost:8000/index.html>

If there is any malfunctioning or unexpected behaviour, double check that you downloaded the required data that are in a separate repository (see previous section). If that does not work, try to clear your browser's cache. If that also does not work, do not hesitate to contact me.

Note that to load any map-related data, you will need a working internet connection.

The webapp has been developed and tested in Google Chrome, so that is the recommended browser.

### License

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
