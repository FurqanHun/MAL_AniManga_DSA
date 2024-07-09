# MAL AniManga DSA

## Description
This is a project for the Data Structures and Algorithms course at the Sindh Madressatul Islam University. The project uses python to scrape data from the [MyAnimeList](https://myanimelist.net/) website and store it in a database. The synopsis from the data is taken as x and genre/page type is then used to train four different machine learning models i.e. Logistic Regression, Decision Tree, Random Forest, Support Vector Machine using four different counting techinques i.e. TF-IDF, Hash Matrix, Count Vectorizer, and n-grams.

Aside form four different machine learning models, the project also uses a deep learning model i.e. Long Short Term Memory (LSTM) to train the data. The LSTM model is trained using the synopsis from the data and the genre and page type of the anime/manga as y. The model is then used to predict the genre of an anime/manga based on the synopsis.

## Disclaimer
My Anime List provides API access to their data and it is recommended to use that or Jaiken's [Jikan](https://jikan.moe/) API to access the data instead of scraping the data from the website. The project is not meant to be used for any commercial purposes and is only meant for educational purposes. The project is not affiliated with My Anime List in any way. Web Scraping was done in order to learn the process of scraping data from a website and to learn the process of using machine learning and deep learning models to train data. Also we made sure to do it in a way that does not put any load on the website. We scrapped the data over the course of two weeks and made sure to not send too many requests at once.

## Contributors
- [Qanii](https://github.com/FurqanHun)
- [Muhammad Yameen](https://github.com/yameen022)

## Special Thanks To
- [MyAnimeList](https://myanimelist.net/) for providing the data.
