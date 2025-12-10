#Pandas with hadj abed samira
#for biochimie Master 1 Tlemcen...09/12/2025
#the project members:
#Nasri wail chams eddine
#Gourari yasmina
#Hachemi douaa
#Ghalmi noudjoud 
#Aissaoui chaimaa


import pandas as pd 

#Données : Séquence ADN, Longeur, Pourcentage de GC 
data ={
"Séquence":["ATGCGTACGTA","GCTAGCTAGGCC","TAGCGCGTAAGT","TACGATCGTA","ATGAAAGGCTT","CGTACGTAGC","TTAACCGGAT"],
"Longueur": [12,12,12,10,11,10,10],
 "Pourcentage GC": [50,66.67,58.33,40,45.45,60,50]
 }


# Création d'un DataFrame (tableau pandas)
df = pd.DataFrame(data)
print("****************Création et affichage****************")

# Affichage du tableau
print ("Tableau des Séquences ADN:")
print(df,"\n\n")

#Opérations sur les tableaux :
print("**************** Opération ****************")


#1) Sélectionner la colonne "Longueur"
longueur = df["Longueur"]
print(longueur,"\n\n")


