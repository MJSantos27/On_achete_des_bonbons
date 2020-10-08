# On_achete_des_bonbons

ALGORITHME <ACHETER_DES_BONBONS>


A <-Argent_de_poche (reel,entier)
B <-prix_bonbon (reel)
C <-Nombre_de_bonbons_acheter (entier)


DÉBUT
   
    ECRIRE ("Entrez votre argent")
    LIRE Argent_de_poche
    
    prix_bonbon (reel) <- 0.85
    Nombre_de_bonbons_acheter (entier) <- 0


    SI Argent_de_poche < prix_bonbon ALORS
    ECRIRE (" Vous devez rentrer minimum 0.85 = 1 bonbons")
    FINSI
 
    
    TANTQUE Argent_de_poche >= prix_bonbon FAIRE
    ECRIRE Argent_de_poche - prix_bonbon
    Argent_de_poche <- Argent_de_poche - prix_bonbon
    ECRIRE Nombre_de_bonbons_acheter  + 1
    Nombre_de_bonbons_acheter  <- Nombre_de_bonbons_acheter  + 1
    FINTANTQUE
    
    ECRIRE " Vous pouvez acheter ", Nombre_de_bonbons_acheter  ,"bonbons"
    
    SI Argent_de_poche = 0 ALORS
    ECRIRE (" Merci Aurevoir ")
    SINON    
    ECRIRE (" Il vous reste ", Argent_de_poche ," Merci Aurevoir ")
    FINSI

FIN

