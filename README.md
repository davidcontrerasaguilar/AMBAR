# AMBAR

Our dataset consists of 3,317,428 ratings from around 31,013 users for 443.921 songs and 27,531 artists. The AMBAR dataset contains
four files described in depth in the following paragraphs.

- user_info.csv. This file contains specific users’ information depicted by the attributes user_id (i.e., the dataset index),
country, continent and gender.
- tracks_info.csv. This file contains information on the music items (i.e., tracks or songs). The attributes in this file are
track_id, artist_id, duration, styles (i.e., the style of music), and category_styles (i.e., music style categories).
- artists_info.csv. This file contains artists’ information. The attributes in this file are artist_id, gender, country, continent, styles (i.e., the style of music), and category_styles (i.e., music style categories).
- ratings.csv. This file contains the users’ music preferences represented by a rating. In particular, the attributes in each tuple are user_id, track_id, and rating.

The full dataset is found in data/AMBAR
