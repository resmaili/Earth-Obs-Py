# Python Visualization for Earth Science Tutorial Scripts.
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/resmaili/EarthSciViz/HEAD)

## About this page
The examples in this repository are described in detail in the book [Python for Remote Sensing Applications in Earth Science: A Practical Programming Guide](https://www.amazon.com/dp/1119606888/ref=cm_sw_em_r_mt_dp_P3MK08TP34QRQM0DV5B5). You may use these examples in your work, but please acknowledge or cite this book if you do not significantly alter or improve upon it.

## Running Notebooks interactively online
You can launch a [binder instance](https://mybinder.org/v2/gh/resmaili/EarthSciViz/HEAD) to run the code interactively online. This does not require a Python installation, but your work will not be saved if you close the browser.

## Running Notebooks on your local machine
First download the contents of the repository on your computer. You do this by clicking the *Code* button on the top right, followed by *download ZIP*. You will need to then uncompress the file. You can also download these

You will need [Anaconda](https://www.anaconda.com/) to run these examples, which you can install following the steps on their website.

The versions and libraries may change over time, so I recommend creating a dedicated Python environment for these examples. To do this, you will need to open the *command line*:
* Windows: Anaconda Prompt
* MacOs/Linux: Terminal

Open your command line program. You will need to navigate to the folder that contains the notebooks using the cd command (change directory). For example, if you are using a Windows machine and saved your code in your Documents folder, it may look like:

```bash
cd C:\Users\your_name_here\Documents\EarthSciViz-master
```

Next, we can setup our environment. This will install all the libraries we need to run the examples. To do this, we use the following command:

```bash
conda env create -f environment.yml
```
This may take a few minutes. After the new environment is created (named earthsciviz), we need to switch to it instead of using our default environment. To do this, type:

```bash
conda activate earthsciviz
```

Lastly, Launch Jupyter Notebooks to view and run the contents interactively. Type the command:

```bash
jupyter notebook
```

This will open a window in your default browser. Navigate to the folder that contains the notebooks (*.ipynb) and click on the tutorial that you wish to run. Any changes you make to these files will be saved to your local machine.

You can end you session by closing the command line program. If you wish to resume at a later time, you will need to again change to the correct directory (via cd ...) reactive the environment (via conda activate...) and launch jupyter notebooks.

## Need more Python help?
### From the author
I will occasionally upload short tutorials to my YouTube channel, [Python for Earth Science](https://www.youtube.com/channel/UCGa4rhczYNTGBYIMxmR8nHg). I also offer a workshop at the American Geophysical Union annual meeting.

### Specific topics (mostly free)
<b> Pandas </b>
* Short Introduction: https://pandas.pydata.org/pandas-docs/stable/getting_started/10min.html
* Cookbook for more details: https://pandas.pydata.org/pandas-docs/stable/user_guide/cookbook.html#cookbook

---
<b> Matplotlib </b>
* Pyplot Tutorial: https://matplotlib.org/3.1.1/tutorials/introductory/pyplot.html

---
<b> Reading self describing file </b>
* <b> NETCDF </b>
    * Detailed tutorial https://unidata.github.io/netcdf4-python/netCDF4/index.html.
* <b> HDF files </b>
    * The package [h5py](https://www.h5py.org/) is similar to netcdf4.
    * User manual at http://docs.h5py.org/en/stable/.
* <b> GRIB/GRIB2 files </b>
    * World Meteorology Association standard format, e.g. commonly used with weather-related models like ECMWF and GFS.
    * Can be opened using [pygrib](https://github.com/jswhit/pygrib).
    * Example usage at https://jswhit.github.io/pygrib/docs/.
* <b> BUFR </b>
    * Another common model format.
    * Open with [python-bufr](https://github.com/pytroll/python-bufr), part of the pytroll project.
---    

### General Python resources   

<b> Free online Tutorials</b>
   * Youtube series for absolute beginners [CS Dojo](https://www.youtube.com/watch?v=Z1Yd7upQsXY&list=PLBZBJbE_rGRWeh5mIBhD-hhDwSEDxogDg)
   * Enhance your workflow [Automate Boring Stuff](https://automatetheboringstuff.com/)

## Problems with Code?
Please submit an issue in the GitHub repository if you encounter any problems. Examples in this repository will always be the most up-to-date version.
