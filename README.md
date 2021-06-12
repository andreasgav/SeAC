# SeAC dataset

We are making publicly available the *Sentiment and Art Class Dataset*, abbreviated as the _SeAC dataset_. Main target of our work was to create an artwork database, as there are limited publicly available resources of art-driven data, for machine learning projects. **SeAC dataset** consists of 14 different art movements, which are namely (in alphabetical order):

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

![image](https://drive.google.com/uc?export=view&id=1wX11VPqS-Pfv0BXsPQJdrZk4JdPVpPcH {width=40px height=400px})

### Data acquisition and availability standards

The paintings as well as the artworks inserted in the database are freely available, so that usage rights and copyright issues do not arise. As a result the available data is copyright free and available for academic and research purposes. The artworks that form SeAC dataset were mainly extracted from _WikiArt online encyclopedia_. WikiArt 250,000 works of art by 3,000 different artists. The overall work available from the site is non-profit. The content of the website is released free of charge by the management team of the website which is based on voluntary participation. Street Art artworks data collection was done through web scraping in the websites maintained by the artists themselves, where the majority of the artists freely shares the works of art they create. Also, as most of these artworks are created on walls of public or private buildings, almost exclusively without any kind of authorization, so they are not under any kind of copyright issues.

### Classification Dataset labeling

Unfortunately we do not provide other information apart from art genre of the painting and the artist that painted the artwork. In this particular work it was necessary to correctly mark the artworks in the fields of origin (artist) and the artistic style that are included. As the majority of the data comes from the WikiArt online repository, it was possible to easily identify the artist, as well as the artistic stream in which each work studied, as WikiArt provides the ability to search the total work of a artist based on different artistic styles. Obviously, this distinction made in the repository does notguarantee the validity of the result, so a further validation/examination of the labels was made based on our personal criterion for the correct labeling of the works used, to ensure the smallest possible amount of mislabelled data. Apparently, it is not possible to thoroughly control a sample of images that exceed 14000 in number. As this work was manual (Web scraping) this resulted to the limited availability of more information for each painting apart from painter and art class.

### One-hot encoding

One-hot encoding technique was chosen in order to classify the artworks into different classes, which is consideredthe best available option for data that do not have an arithmetic but a categorical value, as for example art genres (Impressionism, Cubism etc). Value 0 was attained to art classes that were not representative of the art artwork characterized and value 1 was attained to the class that suited best the artcriteria to classify the painting into a specific category. It is noted that it is possible to have more than one  positive values (1) for one artwork, in the case that it fulfills the criteria to be characterized as both Cubism and Surrealism for example, but in this work we chose to have only one positive value in each artwork, in order to produce highlydiscrete data.

### Emotion Dataset labeling

The collection of labels was chosen to result from human observers, who were not professional art historians. The annotated labels resulted from a specially designed questionnaire that was filled from 67 participants. Almost all participants were aged between 18-35. Each participant was asked to choose from a pre-chosen set of emotions that best fitted his/her emotional state while looking at a given artwork from SeAC dataset. The pre-chosen emotions were the 6 following:

- Joy
- Sadness
- Disgust
- Surprise
- Anger
- Fear

The selection of these emotions was based on Ekman’s distinctive model. To ensure that the resulting dataset will have sufficient data for deep learning models, it was considered necessary for each artwork to be annotated by three different annotators. As a result of this logic, three distinct datasets of emotion emerged, for the same artwork database. This ensures that deep learning models that will be trained on SeAC dataset and perform satisfactorily in all three sets of data are really emotion-oriented and did not accidentally fit into a particular label dataset.

### Artworks Links:

Artworks of SeAC dataset are available in the following three links (you will be warned if you are sure if you want to download the files, but do not worry as it is automated message to any file that exceeds 25 Mb). We provide the artworks of the dataset, in three different parts, in alphabetical order.

[Painter names A - C - download link](https://drive.google.com/uc?id=18gJZGRthEA_5Z0A5uADs63K7a2r1NcVL&export=download)

[Painter names D - R - download link](https://drive.google.com/uc?id=1UJnC6yrn8-Cqa84thhGVu8Si8Ewr5rJr&export=download)

[Painter names S - W - download link](https://drive.google.com/uc?id=1_rPloziapuBjQbJvKJK4YXAeKzjwjzc-&export=download)

### Labels links:

We provide 4 different sets of labels. The first corresponds to image classification projects and the last 3 to sentiment analysis projects.

[Classifications Labels - download link](https://drive.google.com/uc?id=1wiKfNeMuVSiQDntwKag6cNGFy3ssm5iq&export=download)

[Emotion labels from first froup of annotators - download link](https://drive.google.com/uc?id=1CyqrSfxCawhI_aLykEmKlCHHaTIYNvCH&export=download)

[Emotion labels from second froup of annotators - download link](https://drive.google.com/uc?id=1LxllELLfjfKmj8VUqdizdE-o99at42im&export=download)

[Emotion labels from third froup of annotators - download link](https://drive.google.com/uc?id=1pCDbqhY_n7oEJwKjfQSOIozg8P17UC0Y&export=download)

## Citation

Although the use of the available resources is free, a citation to the creators of the dataset is considered necessary. So if SeAC dataset is used as a whole or as a part of a project, you should include the following citation:

Gavros, A., Demetriadis, S. and Tefas, A. _A dataset dor sentiment and art movement classification of paintings._ (2021)
