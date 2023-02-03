# projet
projet meteo
enzo edmond
erwane nouwop
groupe 1


le projet contient une commande "help" qui explique à l'utulisateur quels sont les commandes que le script peut executer: ./meteo.sh --help
pour executer le programme il faut une commande (-t/-p/-w/-m) accompagné d'un mode '1/2/3',
accompagné de -i 'meteo.csv'(fichier d'entrée) -o 'sortie.csv'(fichier de sortie) auxquelles on rajoute (-A/-G/-F/-S/-Q/-O) pour la zone géographique.
les commandes -g/-a/-d ne sont pas fonctionels.

le programme C va receuillir et vérifier chaque argument.
Si un argument n'est pas bon le programme affichera une erreur demandant à l'utilisateur de rentrer des arguments valides.

Si les arguments sont corrects le programme C va passer tous le fichier sous forme de tableau... ce qui va prendre un petit peu de temps...
Il ne gardera que les dates, les Id de stations, et les donner qui auront été rentrer en arguments.
les donnés seront triés selon le mode choisi (1,2 ou 3)
les données seront ensuite écrites dans le fichier rentrer en -o :sortie csv
il va ensuite "tenter de construire" un graphique basés sur les données demandés, cependant l'utilisation de gnuplot a été laborieuse...
les graphiques rentrés ne sont pas corrects nous avons laissé le gnutest comme preuve de notre tentative.
une image png est alors créée parmi les fichiers, seuls les graphiques concernant les pressions et les températures (-t/-P) sont fonctionnels.
selon les arguments choisi le programme met entre 150 set 1200 secondes à s'executer...

exemples de commandes valides :
./meteo.sh -p '1' -i 'meteo.csv' -o 'sortie.csv' -G 
./meteo.sh -t '1' -i 'meteo.csv' -o 'sortie.csv' -G
./meteo.sh -p '2' -i 'meteo.csv' -o 'sortie.csv' -A 
./meteo.sh -t '3' -i 'meteo.csv' -o 'sortie.csv' -S  



