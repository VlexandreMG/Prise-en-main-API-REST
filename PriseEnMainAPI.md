# 4339 et 3914

## Livre 
| Verbe | Operation             | URI     | Code retour | Corps  |  
| ------| --------------------- | ------- | ----------- |--------|
| GET   | Lire tous les livres  | /livres | 200         |        |
| GET   | Lire un livre         | /livres/{id} | 200    |        |
| POST  | Créer un livre        | /livres | 201         | {titre : "Mitaraina ny tany" , idAuteur : 1 };|
| PATCH | Modifier un livre     | /livres/{id} | 200 ou 204 | {titre : "Bobo"}; |
| DELETE | Supprimer un livre   | /livres/{id} | 200 ou 204 |    |
| GET   | Filtrer par auteur    | /livres?auteur=1 | 200  |    |
| GET   | Pagination            | /livres?page=2   | 200  |      


## Auteur 
| Verbe | Operation              | URI      | Code retour | Corps  |
| ------| ---------------------- | ---------| ----------- | -------|
| GET   | Lire tous les auteurs  | /auteurs | 200         |        |
| GET   | Lire un auteur         | /auteurs/{id} | 200    |        |
| POST  | Créer un auteur        | /auteurs | 201         | {nom : "RAHARIMIRANTY" , prenom : "Gaëlle" , date_debut : "2026-05-05" , date_fin : "2026-05-12"};|
| PATCH | Modifier un auteur     | /auteurs/{id} | 200 ou 204 | {nom : "Rojo"}; |
| DELETE | Supprimer un auteur   | /auteurs/{id} | 200 ou 204 |    |
| GET   | Filtre par nom         | /auteurs?nom="DOX" | 200     |    |
| GET   | Filtre par prenom      | /auteurs?prenom="Gaëlle" | 200     |    |
| GET   | Filtre par date         | /auteurs?date_debut=2026-05-02&date_fin=2026-05-10 | 200     |    |
| GET   | Pagination            | /auteurs?page=2   | 200  |      


## Adherents 
| Verbe | Operation                | URI        | Code retour | Corps  | 
| ------| ------------------------ | ---------- | ----------- |------- |
| GET   | Lire tous les adherents  | /adherents      | 200         |        |
| GET   | Lire un adherent         | /adherents/{id} | 200    |        |
| POST  | Créer un adherent        | /adherents      | 201         | {nom : "Vanella" , prenom : "Elia" , naissance : "2026-05-05" };|
| PATCH | Modifier un adherent     | /adherents/{id} | 200 ou 204 | {nom : "Huhu"}; |
| DELETE | Supprimer un adherent   | /adherents/{id} | 200 ou 204 |    |
| GET   | Filtre par nom         | /auteurs?nom="juju" | 200     |    |
| GET   | Filtre par prenom      | /auteurs?prenom="sheee" | 200     |    |
| GET   | Filtre par date         | /auteurs?naissance=2026-05-02 | 200     |    |
| GET   | Pagination            | /adherents?page=2   | 200  |      


## Emprunts 
| Verbe | Operation             | URI       | Code retour | Corps  |
| ------| --------------------- | --------- | ----------- | ------ |
| GET   | Lire tous les emprunts| /emprunts | 200         |        |
| GET   | Lire un emprunt         | /emprunts/{id} | 200    |        |
| POST  | Créer un emprunt        | /emprunts | 201         | {livre : "huhu" , adhérent : "balou" };|
| PATCH | Modifier un emprunt     | /emprunts/{id} | 200 ou 204 | {idLivre : 2}; |
| DELETE | Supprimer un emprunt   | /emprunts/{id} | 200 ou 204 |    |
| GET   | Filtre par nom         | /emprunts?livre="juju" | 200     |    |
| GET   | Filtre par prenom      | /emprunts?adhérent="balou" | 200     |    |
| GET   | Pagination            | /emmprunts?page=2   | 200  |      
