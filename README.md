# Exploring CMIP6 Climate Data and Surface Temperature Cookbook

<img src="thumbnails/thumbnail.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)



This Project Pythia Cookbook covers how to access, analyze, and visualize CMIP6 climate model data using Python tools such as Intake-ESM, Xarray, and Cartopy.

## Motivation

This cookbook was created to help students learn how to work with CMIP6 data. It enables students to remotely query, open, and visualize large CMIP6 datasets without downloading terabytes of data.

## Authors

[Zakara Drakes](https://github.com/zakara1)

## Structure

Notebook Directory:

Notebook 1: Exploring CMIP6 Climate Data
- Purpose:
  Demonstrates how to discover and load CMIP6 data using the Intake-ESM catalog.

- Key Steps:
    - Access the CMIP6 catalog via intake-esm.
    - Filter datasets by variable, experiment, and model.
    - Explore metadata (dimensions, coordinates, attributes).
    - Convert queried collections to xarray.Dataset objects.

- Learning Outcome:
  Understand how to query, filter, and access cloud-optimized CMIP6 data using Pangeo tools.

Notebook 2: Exploring CMIP6 Surface Temperature
- Purpose:
  Builds on the first notebook to analyze near-surface air temperature (tas).

- Key Steps:
    - Load model data for tas under a historical scenario.
    - Compute climatological means and anomalies.
    - Visualize spatial patterns using cartopy and matplotlib.
    - Interpret global warming trends and temporal variations.

- Learning Outcome:
  Learn to subset, aggregate, and visualize CMIP6 temperature fields to assess model behavior.

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/Exploring-CMIP6-Climate-Data-and-Surface-Temperature-Cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/Exploring-CMIP6-Climate-Data-and-Surface-Temperature-Cookbook.git
   ```

1. Move into the `Exploring-CMIP6-Climate-Data-and-Surface-Temperature-Cookbook` directory
   ```bash
   cd Exploring-CMIP6-Climate-Data-and-Surface-Temperature-Cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate Exploring-CMIP6-Climate-Data-and-Surface-Temperature-Cookbook
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
