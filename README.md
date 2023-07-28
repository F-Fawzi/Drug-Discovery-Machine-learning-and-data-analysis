# Drug-Discovery-Machine-learning-and-data-analysis
Un projet de bio-informatique pour la découverte de médicaments (Données de la base de données ChEMBL) en utilisant: Python et l'apprentissage automatique pour construire un modèle. Le target protein est : L'acétylcholine.

### Part 1 :  


### Part 2 :  
Chargement des données preprocess   
Calcul de Lipinski descriptors :  
La règle de cinq de Lipinski est un concept fréquemment utilisé dans la découverte de médicaments. Cette règle permet de prédire si une molécule biologiquement active est susceptible d'avoir les propriétés chimiques et physiques pour être biodisponible par voie orale. La règle de Lipinski fonde les propriétés pharmacocinétiques des médicaments telles que l'absorption, la distribution, le métabolisme et l'excrétion sur des propriétés physicochimiques spécifiques telles que :
1.	Pas plus de 5 donneurs de liaisons hydrogène
2.	Pas plus de 10 accepteurs de liaisons hydrogène
3.	Masse moléculaire inférieure à 500 Da
4.	Coefficient de partage inférieur à 5
Selon la règle de cinq de Lipinski, un médicament actif par voie orale ne peut avoir plus d'une violation de ces conditions.
Source : https://dev.drugbank.com/guides/terms/lipinski-s-rule-of-five

### Part 3 :
Dans la troisième partie, on va calculer les discripteurs molèculaire et les empreintes digitales. 

# Terms Definition
* L'acétylcholine est un messager chimique qui transmet des signaux entre les nerfs et les muscles. Une enzyme appelée acétylcholinestérase décompose l'acétylcholine. Certains médicaments utilisés pour traiter la myasthénie grave agissent sur l'acétylcholinestérase pour arrêter la dégradation de l'acétylcholine.
* Médicament : un médicament est une entité biologique ou chimique qui peut moduler l'évolution d'une maladie en interagissant avec sa protéine cible.  
* Les enzymes sont des protéines (ou parfois des acides ribonucléiques) dont le rôle est de catalyser les réactions chimiques du vivant.  
* Entité biologique: les anticorps.    
* Entité chimique:petites molécules.      
Hits : les séquences identifiées, se sont les séquences qui sont similaires ou identiques aux requêtes du dépistage cellulaire haut débit.  
Leads : sont des composés qui ont fait l'objet d'optimisations structurelles mineures à partir de hits. À partir de là, Ils sont souvent soumises à d'autres séries d'optimisations.  
* Quels sont les test non paramétrique ?  
Un test non paramétrique est un test d'hypothèse qui n'exige pas que la distribution de la population soit caractérisée par certains paramètres. Par exemple, de nombreux tests d'hypothèse supposent que la population obéit à une loi normale pour les paramètres µ et σ.  
* Le test Mann-Whitney U évalue si deux groupes échantillonnés sont susceptibles de provenir de la même population et demande essentiellement; ces deux populations ont-elles la même forme en ce qui concerne leurs données ? En d'autres termes, nous voulons des preuves quant à savoir si les groupes sont tirés de populations avec différents niveaux d'une variable d'intérêt. Il s'ensuit que les hypothèses d'un test U de Mann-Whitney sont :  
L'hypothèse nulle (H0) est que les deux populations sont égales.  
L'hypothèse alternative (H1) est que les deux populations ne sont pas égales.

# Bibliothèques python :  
* RDKIT : RDKit est une bibliothèque open-source pour cheminformatics. Rdkit package ne prend en charge que l'installation conda. La majorité des fonctionnalités chimiques «de base» (par exemple, lecture / écriture de molécules, recherche de sous-structures, nettoyage moléculaire, etc.) se trouvent dans le rdkit.Chemmodule. Les fonctionnalités plus avancées ou moins fréquemment utilisées se trouvent dans rdkit.Chem.AllChem. pour plus d'informations veuillez voir ce site  (https://xinhaoli74.github.io/blog/rdkit/2021/01/06/rdkit.html).  
* PaDEL-Descriptor est un logiciel de calcul de descripteurs moléculaires et d'empreintes digitales. Le logiciel calcule actuellement 797 descripteurs (663 descripteurs 1D, 2D et 134 descripteurs 3D) et 10 types d'empreintes digitales. Ces descripteurs et empreintes digitales sont calculés principalement à l'aide de The Chemistry Development Kit. Certains descripteurs et empreintes digitales supplémentaires ont été ajoutés, notamment des descripteurs d'état électrotopologique de type atome, le volume de McGowan, des descripteurs de relation d'énergie libre linéaire moléculaire, le nombre d'anneaux, le nombre de sous-structures chimiques identifiées par Laggner, et les empreintes digitales binaires et le nombre de sous-structures chimiques identifiées par Klekota et Roth.  
Source : https://onlinelibrary.wiley.com/doi/full/10.1002/jcc.21707?scrollTo=references


Source : https://github.com/dataprofessor/code
