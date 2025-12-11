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

#2) Filtrer les séquences dont la longueur supérieure à 10
print("**************** Filtrage dont la longueur ****************")
# Filtrer les séquences dont la longueur supérieure à 10 
filtred_df = df[df["Longueur"] > 10]
print(filtred_df,"\n\n")

#3) calculer la moyenne du pourcentage de GC
print("****************calcul de la moyenne****************")
# calculer la moyenne du pourcentage de GC 
average_gc=df["pourcentage ].mean()
print(f"pourcentage moyen de GC :{average_gc:.3f}%","\n\n")

#4) Ajouter un nouvelle colonne avec des calculs print("****************Ajouter d'une nouvelle colonne****************") 
# Ajouter un nouvelle collone "Catégorie GC" df["Catégorie GC"]=df["Pourcentage GC"].apply(lambda x: "Riche" if x >55 else "Moyen" if 45< x <55 else "Faible" print(df,"\n\n")

#5) Ajouter une colonne comptant les 'G'
df["Nombre de G"] = collone["Séquence"].str.count("G")
print("===== Nombre de G ajoutés =====")
print(df,"\n\n") 
