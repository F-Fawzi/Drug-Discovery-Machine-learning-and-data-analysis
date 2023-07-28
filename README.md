# Drug-Discovery-Machine-learning-and-data-analysis
Un projet de bio-informatique pour la découverte de médicaments (Données de la base de données ChEMBL) en utilisant: Python et l'apprentissage automatique pour construire un modèle.  

Part 1 :  


Part 2 :  
# Chargement des données preprocess   
# Calcul de Lipinski descriptors :  
La règle de cinq de Lipinski est un concept fréquemment utilisé dans la découverte de médicaments. Cette règle permet de prédire si une molécule biologiquement active est susceptible d'avoir les propriétés chimiques et physiques pour être biodisponible par voie orale. La règle de Lipinski fonde les propriétés pharmacocinétiques des médicaments telles que l'absorption, la distribution, le métabolisme et l'excrétion sur des propriétés physicochimiques spécifiques telles que :
1.	Pas plus de 5 donneurs de liaisons hydrogène
2.	Pas plus de 10 accepteurs de liaisons hydrogène
3.	Masse moléculaire inférieure à 500 Da
4.	Coefficient de partage inférieur à 5
Selon la règle de cinq de Lipinski, un médicament actif par voie orale ne peut avoir plus d'une violation de ces conditions.
Source : https://dev.drugbank.com/guides/terms/lipinski-s-rule-of-five


# Terms Definition
Médicament : un médicament est une entité biologique ou chimique qui peut moduler l'évolution d'une maladie en interagissant avec sa protéine cible.  
*Les enzymes sont des protéines (ou parfois des acides ribonucléiques) dont le rôle est de catalyser les réactions chimiques du vivant.  
*Entité biologique: les anticorps.    
*Entité chimique:petites molécules.      
Hits : les séquences identifiées, se sont les séquences qui sont similaires ou identiques aux requêtes du dépistage cellulaire haut débit.  
Leads : sont des composés qui ont fait l'objet d'optimisations structurelles mineures à partir de hits. À partir de là, Ils sont souvent soumises à d'autres séries d'optimisations.  

Bibliothèques python :  
*RDKIT : RDKit est une bibliothèque open-source pour cheminformatics. Rdkit package ne prend en charge que l'installation conda. La majorité des fonctionnalités chimiques «de base» (par exemple, lecture / écriture de molécules, recherche de sous-structures, nettoyage moléculaire, etc.) se trouvent dans le rdkit.Chemmodule. Les fonctionnalités plus avancées ou moins fréquemment utilisées se trouvent dans rdkit.Chem.AllChem. pour plus d'informations veuillez voir ce site  (https://xinhaoli74.github.io/blog/rdkit/2021/01/06/rdkit.html).



Source : https://github.com/dataprofessor/code
