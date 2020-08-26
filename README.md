# On_achete_des_bonbons

A = Argent de poche 
B = prix bonbon
C = Nombre de bonbons acheter


DÉBUT
   
    ECRIRE "Entrez votre argent"
    LIRE A
    B = 0.85
    C = 0


    SI A < B ALORS
    ECRIRE " Vous devez rentrer minimum 0.85 = 1 bonbons"
    FINSI
 
    
    TANTQUE A >= B FAIRE
    ECRIRE A - B
    A = A - B
    ECRIRE C + 1
    C = C + 1
    
    

    FINTANTQUE
    
    ECRIRE " Vous pouvez acheter ",C ,"bonbons"
    
    SI A = 0 ALORS
    ECRIRE " Merci Aurevoir "
    SINON    
    ECRIRE " Il vous reste ",A," Merci Aurevoir "
    FINSI

FIN

