# projet_ic

Ce dépôt Git contient uniquement les fichiers que nous avons modifiés. Le projet complet, incluant l'ensemble du code source, des dépendances et des ressources, est hébergé sur Google Drive.

## Structure du dépôt Git

Nous avons intégré ici les 3 fichiers spécifiques que nous avons modifiés :
1. `Create_dataset_robin.ipynb` : [Permet de créer le dataset en partant des images médicale (simu ou vivo) dans le format d'entrée du modèle]
2. `Resultats.ipynb` : [Permet de visualiser et avoir les métrique des résultats]
3. `projet_ic_robin.ipynb` : [Mets en place l'environement avec les bonnes dépendances puis lance le code pour utiliser le modèle en inférence. Ce code est à lancer sur les A100 ou un architecture qui support torch 1.13.]

## Installation et Accès

1. **Accéder au projet complet** : Pour avoir l'intégralité du projet via ce lien Drive : [[Lien vers drive](https://drive.google.com/drive/folders/1k4WcHOlmDnR-V2i44y0tGx6PK4E9Kl_L?usp=sharing)].

## Exécution des Expériences

Pour lancer plusieurs expériences, des manipulations supplémentaires peuvent être nécessaire :
* Vous pouvez modifier le fichier de script situé sur le Drive : `projet_robin/scripts/sr_val_ddpm_text_T_vqganfin_old.py`. Le changement faisable dans ce fichier est pour mettre ou non la sortie de la classification de bateau à 0.
* Dans le fichier projet_ic_robin.ipynb en changeant le nom du fichier dans le --config, l'exemplde base est : configs/shipinsight/v2-finetune_text_T_512.yaml. Mais les alternatives possibles pour les fichiers de configs sont configs/shipinsight/v2-finetune_text_T_512{name}.yaml, avec name qui peut-être vivo ou simu. Cela permet de prendre les configurations avec les changements de prompt pour avoir l'embedding de CLIP.

## Contact

Si vous avez des questions concernant l'accès au Drive ou la structure des fichiers modifiés, n'hésitez pas à nous contacter.
