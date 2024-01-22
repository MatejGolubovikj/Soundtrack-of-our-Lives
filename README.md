# Age aware recommendation

This repository holds the data and code used for the Age aware recommendation experiment in the paper "Anonymous Authors, Soundtracks of Our Lives: How Age Influences Musical Preferences", for the purpose of experiment reproducibility (the paper is currently going through a double-blind review process and therefore authors are omitted). The experiment was implemented in Python 3 using Jupyter Notebooks and the recommender systems toolkit LensKit.

## Data

For the purpose of the experiment we use a sample of users, tracks and listening events (LEs) taken from the LFM2b dataset ("http://www.cp.jku.at/datasets/LFM-2b/"). The samples of users, tracks and LEs necessary for the experiment are included in the repository with this notebook. For more information on the sample, we point the reader to the aforementioned paper.

## Requirements

The experiment was run in Python 3 using Jupyter Notebooks and depends on a number of libraries. Most of the requirements are available in the Anaconda distribution (https://www.anaconda.com/download). Only the LensKit library is not present in the anaconda distribution and needs to be installed separately (https://lkpy.readthedocs.io/en/stable/install.html). The full list of dependencies is:

- Python v3.11.5 ("https://www.python.org/downloads/"),
- Jupyter Notebook v6.5.4 (https://jupyter.org/) - browser-based python notebooks, 
- Pandas v1.5.3 (https://pandas.pydata.org/) - data wrangling library, 
- NumPy v1.24.3 (https://numpy.org/) - linear algebra library,
- LensKit v0.14.2 (https://lenskit.org/) - recommender system library.

## Files
Present are the following files:

- Age Modeling Evaluation Experiment.ipynb - a jupyter notebook file, written in python 3, detailing the procedure of the experiment. This file holds both the code and documentation of the procedure.
- full_training_subset_of_select_tracks_experiment.parquet - Our sample of listening event used in the experiment. Stored in .parquet file format which can be read by the Pandas library.
- tracks_artist_index_for_experiment.parquet -  Our sample of tracks used in the experiment along a record for the artist for each track. Stored in .parquet file format which can be read by the Pandas library.
- user_age_index_basic_for_experiment_updated.parquet -  Our sample of user used in the experiment along a record for users' age. Stored in .parquet file format which can be read by the Pandas library.