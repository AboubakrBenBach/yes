#!/bin/bash


while true
clear
do
	
        printf "                   BIENVENU SUR MON PROJET SYS \n         "
         

         echo -e "\n"
         echo "                            MENU"
         echo -e "\n"

	 echo "1. Information sur des utilisateurs integrés il y'a 3jours"
	 echo "2. Acquisition,installation et lancement de l'environnement Xampp"
	 echo "3. Archivage des elements du repertoire personnel qui ont été modifié par l'utilisateur sudoer il y'a 2 jours dans un peripherique externe"
	 echo "4.Informations sur l'utilisation du disque,de la memoire,du processeur et de la swap"
	 echo " q) Quitter !!! "

	 echo -e "\n"
	 echo -e "Veuillez choisir une action \c "
	read reponse

	case "$reponse" in 
		  1)
        #la commande qui permet de donner des informations sur des utilisateurs connecté 3 jours
		    last seed -3;;
		 
		  2) 

        #la commande qui permet le telechargement de xampp
                    wget https://www.apachefriends.org/xampp-files/7.0.18/xampp-osx-7.0.18-0-installer.dmg;
                    echo "telechargement terminé"

        #la commande qui donne le droit de lecture,ecriture et execution
                    sleep 2
		    sudo chmod 755 xampp-linux-*-installer.run;

        #la commande qui permet l'installation
                    sleep 2
		    sudo ./xampp-linux-*-installer.run;
                    echo "installation terminée"


        #la commande qui permet le lancement de xampp
		    sudo /opt/lampp/lampp start ;;

		  3)
                    tar cvf archive.tar ~;;
		 
		  4)

        #la commande qui donne des informations sur l'utilisation du disque,lamemoire, du processeur et de la swap
                    vmstat ;;

		  #ça permet de quitter le programme
		 q)
                   echo "Au revoir"
                   exit ;;
  	esac
        echo -e " Cliquer sur enter pour continue.... \c\n"
     read input
done		
