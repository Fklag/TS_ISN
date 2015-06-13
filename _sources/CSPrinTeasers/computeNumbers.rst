..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".

..  shortname:: Chapter: What You Can Do with a Computer
..  description:: Some tidbits of what you can do with a computer

.. setup for automatic question numbering.

.. 	qnum::
	:start: 1
	:prefix: Q


.. |runbutton| image:: Figures/run-button.png
    :height: 20px
    :align: top
    :alt: run button

.. |audiobutton| image:: Figures/start-audio-tour.png
    :height: 20px
    :align: top
    :alt: audio tour button

.. |teachernote| image:: Figures/apple.jpg
    :width: 26px
    :align: bottom
    :alt: teacher note

Programmer avec des nombres
---------------------------

Dans la suite, vous pourrez executer et modifier des programmes qui fonctionnent avec des mots, des tortues (virtuelles) et des images.

..	index::
	single: variable
	pair: programming; variable
	
Les ordinateurs ont été utilisés d'abord pour les calculs (comme une calculatrice), mais les enchaînements d'opérations sont souvent plus faciles si vous pouvez nommer les valeurs numériques avec lesquelles vous travaillez. Lorsque vous nommez un certain nombre, ou le résultat d'un calcul, vous créez une **variable**. Une variable est un nom associé à la mémoire de l'ordinateur qui peut contenir une valeur et cette valeur peut changer ou varier. Par exemple, le score dans un jeu est une variable : le score initialisé à :math:`0` augmente à mesure que vous jouez.

.. figure:: Figures/pongScore.png
    :width: 400px
    :align: center
    :alt: A game in Scratch with a score
    :figclass: align-center
    
    Figure 2: Un jeu de pong avec |scratch| et l'affichage du score en haut à gauche.

.. |scratch| raw:: html

   <a href="http://scratch.mit.edu" target="_blank">Scratch</a>
       
Dans un premier programme, voyons comment calculer l'indice de masse corporelle (IMC) c'est une mesure standard pour évaluer les risques liés au surpoids chez l'adulte.

* Un IMC de 18,5 ou moins est considéré comme **insuffisant**.
* Un IMC entre 18,5 et 25 est considéré comme **normal**.
* Un IMC entre 25 et 30 est considérée comme **surpoids**.
* Un IMC de 30 ou plus est considéré comme **obèse**.

Pour calculer l'IMC, on doit diviser le poids (en kilos) de l'individu par la taille (en mètres) au carré.

Dans l'encadré ci-dessous, un programme informatique calcule l'IMC pour quelqu'un de 1,70 m et 70 kg.

Appuyez sur le bouton |runbutton| d'exécution ci-dessous pour faire exécuter par l'ordinateur ces étapes. La sortie de ce programme sera affichée dans la colonne de droite.

Pour utiliser les boutons *Save* et *Load*, il faut-être connecté. Le bouton *Save* enregistre le programme en cours et le bouton *Load* va charger un programme sauvegardé.

.. activecode:: IMC
    :nocodelens:
    
    taille = 1.70    # en mètres
    poids = 70   # en kilos
    TailleCarre = taille * taille
    IMC = poids / TailleCarre
    print("IMC:")
    print(IMC)


Changer le poids (en kilos) et la taille (en mètres) dans le programme ci-dessus, et appuyez sur le bouton *Exécuter* pour calculer une nouvelle IMC. 

.. Note
   Notice how naming the values (using variables) for height and weight makes it easier to figure out what values need to be changed.  

.. mchoicemf:: 1_2_1_IMC_Q1
   :answer_a: 18.9
   :answer_b: 18.9919649379
   :answer_c: 19
   :answer_d: 19.0
   :correct: b
   :feedback_a: C'est un résultat tronqué, l'ordinateur affichera plus de décimales.
   :feedback_b: Oui !
   :feedback_c: Non, le résultat est un nombre décimal avec une partie entière et une partie décimale.
   :feedback_d: Non, le résultat affiché par l'ordi n'est pas arrondi.
   
   Imaginez que pour 1,85 m vous êtes à 65 kilos. Quel est votre IMC?


