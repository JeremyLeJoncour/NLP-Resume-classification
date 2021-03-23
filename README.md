# NLP Resume classification

Les deux notebooks propose un modèle de Logistic-Regression avec deux datasets différents. Le premier dataset contient des doublons qui peuvent se retrouver autant dans le train_set que dans le test_set, ce qui peut biaiser la précision du modèle sur les données Test.
Nous avions en effet une accuracy de 99.5%. Ces doublons permettaient d'avoir un modèle plus robuste que sans (où après suppression des données répliquées, nous avions 53% d'accuracy).

![Ressources/Matrice 1.png]

Des tests ont été effectués sur des CV et descriptifs de métier récoltés sur internet qui se rapproche des différentes catégories du dataset initial. Les résultats semblent malgré tout concluant.

![Ressources/Matrice 2.png]

Le deuxième notebook part sur un dataset différent. Après extraction du texte de divers fichiers (txt, pdf, word...) avec python Tesseract, nous avons formé un modèle atteingnant une précision de 65%.

## Conclusion

D'autres modèles pourront être utilisés (RandomForest...) afin de trouver le plus performant pour ce dernier dataset.
