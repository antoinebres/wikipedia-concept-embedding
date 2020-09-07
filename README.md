# wikipedia-concept-embedding

Ce projet a pour but de produire un embedding des concepts informatiques des pages wikipedia.  
Il exploite la structure de wikipedia : Un article reference d'autres articles parlant de concepts proches. Des pages concernant des concepts proches auront des liens en commun.  
Le reseau de neurones aura pour objectif de predire si un lien est present dans une page donnée.  
Normalement, la representation vectorielle apprise capturera des relations pertinentes entre les concepts.  

Ce projet:
- telecharge le dernier wikidump fr
- recupère les pages contenant une de ces Infoboxes : "Langage de programmation", "Logiciel", "Système d'exploitation"
- entraine un nn pour predire si un lien est present dans un article
- sauvegarde le modele entrainé et les embedding

On récupère ainsi deux embeddings (ceux des liens et ceux des pages).
