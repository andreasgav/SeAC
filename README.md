# SeAC dataset

We are making publicly available the *Sentiment and Art Class Dataset*, abbreviated as the SeAC dataset. Main target of our work was to create an artwork database, as there are limited publicly available resources of art-driven data, for machine learning projects. **SeAC dataset** consists of 14 different art movements, which are namely (in alphabetical order):

- Art Nouveau
- Baroque
- Cubism
- Impressionism
- Italian Renaissance
- Mannerism - Late Rennaissance
- Northern Renaissance
- Pop Art
- Post-Impressionism
- Realism
- Rococo
- Romantism
- Street Art
- Surrealism

We made an effort to collect sufficient resources for each genre that we considered representative of the art evolution during the last 600 years, which is considered as modern-day art (after the Middle Ages). The structure of this specific dataset gives emphasis mainly in art movements, whilst the majority of similar databases are structured around painter diversity. SeAC is an image dataset consisting of artworks (exclusively paintings) from 14th to 21st century.

This dataset is orientated on machine learning projects that focus on classification of art movement and sentiment analysis (arousing of certain emotions that result from the sight of a painting). The dataset is formed from 14917 artworks in total, although we are considering an increase in art genres and labels consequently, in the near future. Total number of artists that represented in the current dataset is 140 and we tried to have the most notable for each art class (Picasso in Cubism, Van Gogh in Post-Impressionism, Salvador Dali in Surrealism, Banksy in Street Art, Andy Warhol in Pop Art, El Greco in Mannerism, Caravaggio in Baroque, etc.). As the total database consists of 14 different art movements, all art classes listed are represented with more than 1000 paintings in order to provide a fairly representative sample for each class. 

Unfortunately we do not provide other information apart from art genre of the painting and the artist that painted the artwork. This results of

## Classification dataset

### Dataset labeling

An important parameter for the successful training of a machine learning model targeting classification among artclasses or painters, is the available data to be properly labeled, in order to avoid inserting in-certainty in the process.Obviously, the more incorrectly labeled data, the lower the ability of a convergent model to generalize the informationit draws from the training procedure, resulting in a model with reduced chances of successful prediction.Depending on the art movements, there is a question if certain works are correctly attributed to artists. A typical case isRembrandt, where the origin of several works that until recently were attributed to him is questioned. Recent researchsuggests that about half of the work that Rembrandt has been credited, is likely to have been produced by his students[26]. Similar examples exist to a greater or lesser extend in other artists and as a result of which the error rate attributedto incorrect data increases further.

In this particular work it was necessary to correctly mark the artworks in the fields of origin (artist) and the artisticstyle that are included. As the majority of the data comes from the WikiArt online repository, it was possible to easilyidentify the artist, as well as the artistic stream in which each work studied, as WikiArt provides the ability to searchthe total work of a artist based on different artistic styles. Obviously, this distinction made in the repository does notguarantee the validity of the result, so a further validation/examination of the labels was made based on the author’scriterion for the correct labeling of the works used, to ensure the smallest possible amount of mislabelled data. As itis understood, it is not possible to thoroughly control a sample of images that exceed 14000 in number. It is also notpossible to assure the inclusion of a particular work in an artistic current, since the classification of artworks in specificartistic classes is a field of controversy even among art historians [27].

### One-hot encoding

One-hot encoding technique was chosen in order to classify the artworks into different classes, which is consideredthe best available option for data that do not have an arithmetic but a categorical value, as for example art genres(Impressionism, Cubism etc). Through the use of one-hot encoding the available art classes are transformed into anumerical form that is easily and fast manipulated by deep neural networks. Value 0 was attained to art classes thatwere not representative of the art artwork characterized and value 1 was attained to the class that suited best the artcriteria to classify the painting into a specific category. It is noted that it is possible to have more than one  positive values (1) for one artwork, in the case that it fulfills the criteria to be characterized as both Cubism and Surrealismfor example, but in this work we chose to have only one positive value in each artwork, in order to produce highlydiscrete data. Thus, binary labels are obtained for each element of the database, which is quite easy to manipulate andrecognize by the model, while at the same time it provides speed to the final training time of the classification model.For the configuration of the labels used in SeAC dataset, spreadsheets were used in which based on the category thatwas confirmed for the painting examined i each case, the value 1 was attributed.


### Artworks Links:

Artworks of SeAC dataset are available in the following three links (you will be warned if you are sure if you want to download the files, but do not worry as it is automated message to any file that exceeds 25 Mb). We provide the artworks of the dataset, in three different parts, in alphabetical order. 

[Painter names A - C - download link](https://drive.google.com/uc?id=18gJZGRthEA_5Z0A5uADs63K7a2r1NcVL&export=download)

[Painter names D - R - download link](https://drive.google.com/uc?id=1UJnC6yrn8-Cqa84thhGVu8Si8Ewr5rJr&export=download)

[Painter names S - W - download link](https://drive.google.com/uc?id=1_rPloziapuBjQbJvKJK4YXAeKzjwjzc-&export=download)

### Labels links:

[Classifications Labels - download link](https://drive.google.com/uc?id=1wiKfNeMuVSiQDntwKag6cNGFy3ssm5iq&export=download)

[Emotion labels from first froup of annotators - download link](https://drive.google.com/uc?id=1CyqrSfxCawhI_aLykEmKlCHHaTIYNvCH&export=download)

[Emotion labels from second froup of annotators - download link](https://drive.google.com/uc?id=1LxllELLfjfKmj8VUqdizdE-o99at42im&export=download)

[Emotion labels from third froup of annotators - download link](https://drive.google.com/uc?id=1pCDbqhY_n7oEJwKjfQSOIozg8P17UC0Y&export=download)

