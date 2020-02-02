# SNT-PIL1  
 Le module PIL permet de créer très facilement l'image représentée ci-contre qui est un rectangle de 100 pixels de largeur et 256 pixels de hauteur, de couleur dégradée du noir (en haut) vers le rouge.

Pour créer une nouvelle image, il faut indiquer :

    le nom de la variable qui « contiendra » cette image 
    l'encodage des couleurs de cette image
        'RGBA' : couleurs avec gestion de la transparence (4 octets)
        'RGB' : couleurs sans gestion de la transparence
        'L' : nuances de gris
        '1' : noir & blanc
    les dimensions en pixels (largeur et hauteur) de cette image (sous forme de tuple - liste non modifiable).

Dans notre exemple, on stockera l'image dans la variable im, avec un encodage couleur en 'RGB' et des dimensions 100 x 256 :  
Recopier le code suivant dans votre fenêtre de programmation.  
![image](https://github.com/Svt-lim/SNT-PIL1/blob/master/module%20PIL1/1.jpg)  
executez le et ouvrez le fichier degrade.jpg  
# Colorier chaque pixel.  
le module PIL permet «d'atteindre» et de modifier directement n'importe quel pixel de l'image grâce à ses coordonnées.

    Les coordonnées d'un pixel de l'image sont sous la forme d'un tuple (x, y).
    Selon l'encodage des couleurs du fichier, il faudra saisir une valeur entière différente pour le pixel correspondant :
        'RGBA' : un quadruplet (r, g, b, a) de valeurs comprises entre 0 et 255
        'RGB' : un triplet (r, g, b) de valeurs comprises entre 0 et 255
        'L' : une valeur g comprise entre 0 et 255
        '1' : une valeur nb comprise entre 0 et 1  

## Illustration : 
la fonction suivante : im.putpixel((3, 1), (255, 0, 0)) a permis "d'agir" sur le pixel de coordonnée (3,1)
![image](http://math.univ-lyon1.fr/irem/Formation_ISN/formation_prog_images/module_PIL/images_module_PIL/Coordonnees_PIL.png)  
# Défi 1 :  
Complétez le programme précédent à partir de la ligne 11 afin d'obtenir l'image d'un rectangle de 100 pixels de largeur et 256 pixels de hauteur, de couleur dégradée du noir (en haut) vers le rouge(en bas). 
Indice0, vous avez besoin de la fonction im.putpixel()  
Indice1, vous avez besoin d'une boucle for parcourant chaque pixels de coordonée x,y et les colorants de plus en plus rouge.  
Indice2, la taille de l'image n'a pas été choisie au hasard. Il y a en tout 255 lignes de pixels de haut en bas chacune devant devenir de plus en plus rouge...    
Indice3, la boucle s'écrit :   
 ![image](https://github.com/Svt-lim/SNT-PIL1/blob/master/module%20PIL1/2.jpg)
        


