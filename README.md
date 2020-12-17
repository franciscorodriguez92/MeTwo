# MeTwo: Machismo and Sexism Twitter Identification dataset


This repo contains the MeTwo dataset, a corpus for the detection of sexism in Twitter. If using this dataset please cite: 

```
@ARTICLE{9281090,
  author={F. {Rodríguez-Sánchez} and J. {Carrillo-de-Albornoz} and L. {Plaza}},
  journal={IEEE Access}, 
  title={Automatic Classification of Sexism in Social Networks: An Empirical Study on Twitter Data}, 
  year={2020},
  volume={8},
  number={},
  pages={219563-219576},
  doi={10.1109/ACCESS.2020.3042604}}
```


For further information, you can check https://ieeexplore.ieee.org/document/9281090

This README file contains: 
1) A brief description of the dataset and labels
2) A description of the file MeTwo.csv
3) Contact information


## 1. The MeTwo Dataset


MeTwo uses Twitter data in Spanish. We propose the following labels to identify sexist expressions and behaviours in Twitter:

+ SEXIST: tweets that underestimate women as a result of their gender, independently of the facet of women that is criticised, and independently of the intentionality and violence.
+ NON_SEXIST: tweets without sexist connotations. In this category, we could find xenophobic or offensive tweets but without sexist attitudes.
+ DOUBTFUL: tweets that could be sexist depending on the context, which can not be inferred from the text in the tweet. In this category we find tweets that would be sexist if they were specifically targeted to women.

MeTwo was labeled based on a majority vote by three annotators trained for this task. In the case of total disagreement, a fourth annotator decided the final label.


## 2. Description of the file


We provide the ID and the annotation in a semicolon seperated file (MeTwo.csv). To obtain the individual tweets, use the Twitter API of your choice and query for the ID's provided. In this file, you'll find two columns, separated by semicolon, with the following information:

+ status_id: id of the tweet.
+ category: one of the three labels.

Example:
```
	1049436217648041985;SEXIST
	1060676161058103297;NON_SEXIST
	1047225018424467457;DOUBTFUL
```

## 3. Contact information

Please feel free to contact me at frodriguez.sanchez@invi.uned.es if you have any questions or you need the messages associated with the ID's.