# NLP Resume classification

Trois Notebooks sont proposés : 
* 1 notebooks fournissant un modèle de **RandomForest** a été réalisé dans un premier temps. Les données ont été modifiées en conséquence pour supprimer les caractères spéciaux (Beautiful Soupe / Tokenizer) et transformées sous Word2Vec. Le modèle possède une précision de 100%. La méthode d'évaluation est effectuée sur les données Test dont certaines sont des doublons qui ont pu être utilisées pour l'entrainement de ce modèle et à donc peu d'importance dans ce cas.

* 2 notebooks propose un modèle de **Logistic-Regression** avec deux datasets différents. Le premier dataset contient des doublons qui peuvent se retrouver autant dans le train_set que dans le test_set, ce qui peut biaiser la précision du modèle sur les données Test comme il a été évoqué précédemment.
Nous avions en effet une accuracy de 99.5%. Ces doublons permettaient d'avoir un modèle plus robuste que sans (où après suppression des données répliquées, nous avions 53% d'accuracy). Des tests ont été effectués sur des CV et descriptifs de métier récoltés sur internet qui se rapproche des différentes catégories du dataset initial. Les résultats semblent malgré tout concluant.

![Matrice 1](https://user-images.githubusercontent.com/73163032/112139713-6a237100-8bd3-11eb-80b4-a954619eb852.png)

Le deuxième notebook part sur un dataset différent. Après extraction du texte de divers fichiers (txt, pdf, word...) avec python Tesseract, nous avons formé un modèle atteingnant une précision de 65%.

![Matrice 2](https://user-images.githubusercontent.com/73163032/112139799-83c4b880-8bd3-11eb-95b3-30f9a0d6c8b1.png)

Des nuages de mots ont aussi été réalisés en amont afin de relever les mots les plus importants pour chaque catégorie (ils sont affichés dans les notebooks).
