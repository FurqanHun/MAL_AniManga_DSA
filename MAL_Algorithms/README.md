# MAL Algorithm Results

## F1 Accuracy Scores

|               | Logistic Regression | Decision Tree          | Random Forest          | Support Vector Machine |
|---------------|---------------------|------------------------|------------------------|------------------------|
| TF-IDF        | 0.56                | 0.49 (2nd test)        | 0.57                   | 0.53                   |
| HM            | 0.78                | 0.73                   | 0.77                   | 0.77                   |
| CV            | 0.56                | 0.51                   | 0.57                   | 0.54                   |
| n-gram        | 0.59                | 0.51                   | 0.55                   | 0.54                   |
| W2V           | NO DATA             | NO DATA                | NO DATA                | NO DATA                |

**LSTM ACCURACY: 0.0655653104186058**

(2nd test) in TF-IDF – Decision tree means that 0.49 is the result of the second run of the code, originally, I got 0.50 but as I accidentally re ran the code so I decided to put the newer result.
W2v having no data means I couldn’t get the results as after waiting for nearly an hour I realized that it could take hrs to get the results	and ion think I could afford running the laptop straight for 58hrs.

### Note:
*I used BOW (Bag of Words) instead of HM (Hashing Vectorizer) not realizing tht BOW and CV (Count Vectorizer) are the same thing, I only realized it after I got the results and was writing the report. After i implemented HM*

*HM = Hashing Vectorizer, CV = Count Vectorizer, W2V = Word2Vec*

## Reasoning for not having higher accuracy

I think that the reason I couldn’t get higher accuracy is due to the diversity in the data, I used the synopsis of a total of 9684 entries (manga, manhwa, manhua, anime) and all of them are known for having a different story which means that their synopsis is going to be way different than each other.
According to internet not having higher accuracy could depend on many factors such as complexity or diversity of data, class imbalance, which I probably had in my data set as manga type outweighed the other ones, and as I read on internet, I did have a higher precision rate.
I also think that the reason I couldn’t get higher accuracy is due to the fact that I didn’t have enough data, I only had 9684 entries which is not enough to train the algorithm to get higher accuracy.

## Experimenting to improve accuracy

To stop the algorithms from being bias towards the dominant category I’m going to try and change the category from the “Type” column to the “Page” column and hope that the algorithm being less bias towards the dominant category would produce more accurate results.

## F1 Accuracy Scores after changing the category

|                  | Logistic Regression | Decision Tree        | Random Forest        | Support Vector Machine |
|------------------|---------------------|----------------------|----------------------|------------------------|
| TF-IDF           | 0.56 --> 0.78       | 0.49 --> 0.73        | 0.57 --> 0.78        | 0.53 --> 0.78          |
| HM               | 0.78 --> 0.78       | 0.73 --> 0.74        | 0.77 --> 0.77        | 0.77 --> 0.77          |
| CV               | 0.56 --> 0.76       | 0.51 --> 0.74        | 0.57 --> 0.78        | 0.54 --> 0.76          |
| n-gram           | 0.59 --> 0.78       | 0.51 --> 0.75        | 0.55 --> 0.78        | 0.54 --> 0.76          |
| W2V              | NO DATA             | NO DATA              | NO DATA              | NO DATA                |

**IMPROVED LSTM ACUURACY: 0.5983479619026184**