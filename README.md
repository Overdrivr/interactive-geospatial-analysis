# Interactive geospatial analysis

A collection of Jupyter notebooks for learning geospatial analysis with Python.

To run those scripts you will need to install the [Jupyter notebook](http://jupyter.org/) application.
If you haven't tried it before, you won't regret it.

Throughout the tutorials, several external API are used
for handling heavy computations and resources.
Without these API, it would not be possible to run those script on a regular desktop machine.
Follow the link and request a key to use their APIs.

External API | API type | Tarification
-----|----------|--------------
[`OAlley`](https://api.oalley.fr/) | isochrone / isodistance / routing | Free during beta
[`Open Street Map`](http://tile.openstreetmap.fr/) | tile layers | Free for fair-use
[`Google Maps`](https://developers.google.com/maps/?hl=fr) | tile layers | Free for personal use

For visualization, the `folium` library, although poorly documented, is great.
It acts as a wrapper on top of leaflet.

## Installation
The following packages are required.

```
pip install requests folium grequests polyline
```

The shapely package is also required in some advanced tutorials.
On Unix and Mac systems, install it with `pip`.
```
pip install shapely
```
On Windows, download the package [here](http://www.lfd.uci.edu/~gohlke/pythonlibs/#shapely) (`cp27` for python 2.7, `cp34` for python 3.4, etc.)
Run the following command where the file was downloaded. (Modify the filename if needed).

```
pip install Shapely-1.5.17-cp35-cp35m-win32
```


## Run it

In the parent directory of this repository, run in a terminal the following command
to open the local web-application.

```
jupyter notebook
```

Navigate inside the repository and click on any of the notebooks (`.ipynb` files) to open it.
Go to  `Kernel` -> `Restart and Run all` to run the entire notebook.

Note that you can run a selected cell again by hitting <kbd>Ctrl</kbd> + <kbd>Enter</kbd>.
This is highly convienient if you have made heavy API calls in the previous cell, but just want to update some parameters visualization in the currently selected cell.


## Disclaimer

I am one of the developpers of [OAlley](https://api.oalley.fr/).
This repository is a summary of my experimentations with the API, of playing around with it.
I hope you will enjoy it just as much.
