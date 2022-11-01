# Dataset Directory

The following structure describes the files in the dataset directory.

```
dataset 
├── EN
│   ├── folds
│   │   └── 5-folds train and test tsv files
│   ├── mide22_en_misinfo_events.csv
│   └── mide22_en_misinfo_tweets.tsv
└── TR
    ├── folds
    │   └── 5-folds train and test tsv files
    ├── mide22_tr_misinfo_events.csv
    └── mide22_tr_misinfo_tweets.tsv
```

`dataset` folder divided into two directories according to the languages named as `EN`, for English tweets, and `TR`, for Turkish tweets, respectively.

Each of the language folder includes `tweets.tsv` and `events.tsv` files, and `folds` directory.

`events.tsv`: Contains 40 misinformation events for the corresponding language, together with some attributes, such as, fact-checking source link, keywords used while tweet crawling, end date and start date of the event, etc.

`tweets.tsv`: Contains all tweets having misinformation label for each language. Header of the file includes Topic, Event, Label, and Tweet ID.

`folds`: This directory includes 5-folds train and test files used in the [paper](https://arxiv.org/abs/2210.05401) when presenting baseline experiments. For example, one can use `tr_train_0.tsv` for training the model and `tr_test_0.tsv` for testing the model.
