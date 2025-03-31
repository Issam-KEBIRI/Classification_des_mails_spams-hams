# Classification des mails spams/hams


![GitHub](https://img.shields.io/github/license/issam-kebiri/Classification_des_mails_spams-hams?color=g&style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/issam-kebiri/Classification_des_mails_spams-hams?color=red&style=for-the-badge)
![GitHub contributors](https://img.shields.io/github/contributors/issam-kebiri/Classification_des_mails_spams-hams?color=yellow&style=for-the-badge)


![GitHub dev_language](https://img.shields.io/badge/Python-yellow?style=flat&logo=python&logoColor=white)
![GitHub dev_language](https://img.shields.io/badge/Nltk-blue?style=flat&logo=solidity&logoColor=white)
![GitHub dev_language](https://img.shields.io/badge/Pandas-6aa84f?style=flat&logo=pandas&logoColor=white)
![GitHub dev_language](https://img.shields.io/badge/Scikit--learn-orange?style=flat&logo=scikit-learn&logoColor=white)



![GitHub Org's stars](https://img.shields.io/github/stars/issam-kebiri?style=social)
![GitHub followers](https://img.shields.io/github/followers/issam-kebiri?style=social)

## About The Project

Le but de ce projet est de réaliser une classification de documents, il consiste à classifier des mails en spams/hams en utilisant plusieurs techniques de Machine Learning, les étapes sont :

- Récolte des données
- Nettoyage et préparation des données
  - Supprimer la ponctuation
  - tokenizer les données
  - Elimination des stop words (mots sans valeurs sémantiquement)
  - réduction de la taille du document en réduissant le nombre de type de mot présent dans le doc (stemming ou lemmatization)
- vectorisation (transformer le text en chiffres)
  - vectorisation contextuelle N grams
  - vectorisation tf-idf
  - Feature Engineering : enrichir les données avec de nouvelles variables ou transformer les variables excitantes
- Construire des jeux de données pour l'entrainement et le test
  - Cross-Validation et méthode K-fold
  - matrice de confusion
- Modèles
  - SVM
  - SVM_CrossValidation
- Évaluation des modèles
  - Métriques de performance : precision, recall et accuracy.
- sélection du meilleur modèle

#### Keywords

Machin Learning, NLP, tokenizer, stemming, lemmatization, vectorisation, N_grams, tf-idf, Feature Engineering, Cross-Validation, k-fold, SVM,

#### Built With

* Python
* Pandas
* re
* nltk


## Packages & Library

```python
import pandas as pd
import re
import string
import nltk
from nltk.corpus import stopwords

```

## Dataset

Le Dataset [SMSSpamCollection.txt](Data/SMSSpamCollection.txt) peut être téléchargé [ici](http://dcomp.sor.ufscar.br/talmeida/smspamcollection/)   
Ce jeu de données contient deux informations principales : le contenu d'un mail, et le label qui définit si le mail est spam/ham

source du Dataset :

**[1]** Almeida, T.A., Gómez Hidalgo, J.M., Yamakami, A. Contributions to the Study of SMS Spam Filtering: New Collection and Results.  Proceedings of the 2011 ACM Symposium on Document Engineering (DOCENG'11), Mountain View, CA, USA, 2011.

**[2]** Gómez Hidalgo, J.M., Almeida, T.A., Yamakami, A. On the Validity of a New SMS Spam Collection.  Proceedings of the 11th IEEE International Conference on Machine Learning and Applications (ICMLA'12), Boca Raton, FL, USA, 2012.

**[3]** Almeida, T.A., Gómez Hidalgo, J.M., Silva, T.P.  Towards SMS Spam Filtering: Results under a New Dataset.   International Journal of Information Security Science (IJISS), 2(1), 1-18, 2013.


## Result
Métriques de performance utilisé : precision, recall et accuracy.    
- Résultats pour le [model SVM](SVM_model.ipynb)
  - precision = 0.966, recall = 0.929, accuracy = 0.986
- Résultat pour le [model SVM_CrossValidation](SVM_model.ipynb)
  - accuracy pour chaque batch = [0.97774587 0.9856425  0.9798995  0.98420675]
  - accuracy totale = 0.9818736539842067
- Résultat pour le [model SVM_TF-IDF](SVM_model.ipynb)
  - precision = 0.993, recall = 0.905, accuracy = 0.987


## License

[GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)

## Contact

📫 How to reach me: issam.eddine.kebiri@gmail.com

🌐 My Portfolio: <https://issam-kebiri.github.io/>

🔗 Project Link: [https://github.com/issam-kebiri/Classification_des_mails_spams-hams](https://github.com/issam-kebiri/Classification_des_mails_spams-hams)
