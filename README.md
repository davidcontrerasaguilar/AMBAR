# AMBAR

Our dataset consists of 3,311,462 ratings from around 31,013 users for 443.921 songs and 30,667 artists. The AMBAR dataset contains
four files described in depth in the following paragraphs.

- user_info.csv. This file contains specific users’ information depicted by the attributes user_id (i.e., the dataset index), country, continent and gender.
- tracks_info.csv. This file contains information on the music items (i.e., tracks or songs). The attributes in this file are track_id, artist_id, duration, styles (i.e., the style of music), and category_styles (i.e., music style categories).
- artists_info.csv. This file contains artists’ information. The attributes in this file are artist_id, gender, country, continent, styles (i.e., the style of music), and category_styles (i.e., music style categories).
- ratings_info.csv. This file contains the users’ music preferences represented by a rating. In particular, the attributes in each tuple are user_id, track_id, and rating. It is important to note that, the ratings are not available on the platform we used in this study, where only the playcounts attribute, which represents the number of times a user has listened to a song, is available. Therefore, we transformed the number of playcounts into a 1-5 Likert scale value.  Then, we transformed the implicit feedback embedded in people's listening histories -- represented by the number of playcounts-- into ratings (i.e. a 1-5 Likert scale value).  Concretely, we computed the complementary cumulative distribution of the listening histories per listener, then assigned a score of five to music items (i.e., the track) located in the first quintile, four to the ones in the second quintile, and so forth. It is important to note that this mapping is based on the assumption that people who have listened more to a particular music item prefer it.

The full dataset is found in data/AMBAR


## How to reproduce the experiments

These notebooks were tested using Python 3.8. A virtual environment is highly recommended.

```shell
python -m venv venv
source ./venv/bin/activate
```

The required packages are:

- tqdm: used for showing progress in some loops.
- numpy: used for data manipulation.
- pandas: used for data manipulation.
- cornac: used for obtaining the recommendations.

These can be installed (alongside some extra packages) using the requirements.txt provided.

```shell
python -m pip install --upgrade pip
python -m pip install -r ./requirements.txt
```

For running the notebooks, Jupyter is required and needs to be installed in the virtual environment (not included in
requirements.txt).

## Cornac

For running cornac on the data provided, use the notebook Cornac.ipynb where the process is explained. Some variables
were provided so it can be adapted to other use cases. The data used for this script is found in data/AMBAR.

## PyCPFair

For running PyCPFair on the data provided, use the notebook PyCPFair.ipynb. The main process is found in the process
section.
The data for this script is separated and based on the full set. This data may be found in data/PyCPFair.

## PFair

For running PFair on the data provided, use the notebook PFair_multiclass.ipynb. The main process is found in the process
section.
The data for this script is separated and based on the full set. This data may be found in data/PFair.

## Terms of usage
Dataset use Research only and strictly non-commercial. 
