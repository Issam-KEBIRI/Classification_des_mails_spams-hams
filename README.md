# Classification des mails spams/hams










![GitHub](https://img.shields.io/github/license/kebiri-isam-dine/Classification_des_mails_spams-hams?color=g&style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/kebiri-isam-dine/Classification_des_mails_spams-hams?color=red&style=for-the-badge)
![GitHub contributors](https://img.shields.io/github/contributors/kebiri-isam-dine/Classification_des_mails_spams-hams?color=yellow&style=for-the-badge)

![GitHub Org's stars](https://img.shields.io/github/stars/kebiri-isam-dine?style=social)
![GitHub followers](https://img.shields.io/github/followers/kebiri-isam-dine?style=social)

## About The Project

Le but de ce projet est de réaliser une classification de documents, il consiste à classifier des mails en spams/hams en utilisant plusieurs techniques de Machine Learning, les étapes sont :

- Récolte des données
- Nettoyage et préparation des données
  - Supprimer la ponctuation
  - Elimination des stop words (mots sans valeurs sémantiquement)
  - Réduction de la taille du document en réduissant le nombre de type de mot présent dans le doc (stemming ou lemmatization)
- Vectorisation (transformer le text en chiffres)
- Construire des jeux de données pour l'entrainement et le test
- Entrainement et évaluation du modèle
- sélection du meilleur modèle

#### Keywords

Machin Learning, NLP, 

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



## License

[GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)

## Contact

📫 How to reach me: kebiri.isam.dine@gmail.com

🌐 My Portfolio: <https://kebiri-isam-dine.github.io/>

🔗 Project Link: [https://github.com/Kebiri-isam-dine/UniversityProjects](https://github.com/Kebiri-isam-dine/Classification_des_mails_spams-hams)
