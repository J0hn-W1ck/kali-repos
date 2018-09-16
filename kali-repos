#!/bin/bash 
#
###################
#CREANDO FUNCIONES#
###################
#
#############################################################################
echo 
f_banner() {
echo -e "\e[0;32m██╗  ██╗ █████╗ ██╗     ██╗    ██████╗ ███████╗██████╗  ██████╗ ███████╗    
██║ ██╔╝██╔══██╗██║     ██║    ██╔══██╗██╔════╝██╔══██╗██╔═══██╗██╔════╝    
█████╔╝ ███████║██║     ██║    ██████╔╝█████╗  ██████╔╝██║   ██║███████╗    
██╔═██╗ ██╔══██║██║     ██║    ██╔══██╗██╔══╝  ██╔═══╝ ██║   ██║╚════██║    
██║  ██╗██║  ██║███████╗██║    ██║  ██║███████╗██║     ╚██████╔╝███████║    
╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝╚═╝    ╚═╝  ╚═╝╚══════╝╚═╝      ╚═════╝ ╚══════╝"
echo -e "\e[0;31mAutor: \e[0;37mJohn-Wick   \e[0;31mVersion: \e[0;37m3.0\e[0;31m   Contacto: \e[0;37mhablemosdehacking@gmail.com\e[0m"
echo
echo
}
##############################################################################
f_auto_apt() {
clear
echo
f_banner
echo -e "\e[0;31m[+]\e[0;37m Comprobando instalacion en \e[0;32m/usr/local/bin\e[0m"
if [ -e /usr/local/bin/auto-apt ]
   then
	echo
	echo -e "\e[0;31m[+]\e[0;37m Lanzando\e[0;32m auto-apt\e[0;37m...\e[0m"
	sudo auto-apt
	sleep 5
	f_menu
   else
	echo
	echo -e "\e[0;31m[+]\e[0;37m No esta instalado \e[0;32mauto-apt\e[0m"
	read -p "[Pulse Enter para volver al menu principal.] "
	f_menu
fi
}
##############################################################################
f_ver_repositorios() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[*]\e[0;37m Repositorios actualmente.\e[0m" $(echo -e "\e[0;32m ")
echo
cat -n /etc/apt/sources.list
echo -e "\e[0;37m "
read -p "[Pulse Enter para volver al menu principal.] "
f_menu
}
##########################################################
f_editar() {
clear
echo
f_banner
echo -e "\e[0;31m[+]\e[0;37m Abriendo source.list\e[0m"; sleep 3
nano /etc/apt/sources.list
clear
f_menu
}
##########################################################
f_actualizar() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[Actualizando Sources.list] \e[0;32mEspere por favor....\e[0m";  sleep 1
echo -e "\e[0;37m "
apt -y update 
echo -e "\e[0;31m "
read -p "[Pulse Enter para volver al menu principal] "
f_menu
}
##########################################################
f_moto() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[+]\e[0;37m Agregando los repositorios y actualizando sorces.list\e[0m"
echo -e "\e[0;31mEspere...\e[0m" ; sleep 5
echo '#KALI LINUX MOTO (1.0)' >> /etc/apt/sources.list  
echo 'deb http://old.kali.org/kali moto main non-free contrib' >> /etc/apt/sources.list
echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
echo '# deb-src http://old.kali.org/kali moto main non-free contrib' >> /etc/apt/sources.list
sudo apt update
echo -e "\e[0;31m[+]\e[0;32m Repsitorios agregados y actualizados correctamente.."
echo -e "\e[0;37m " $(echo -e "\e[0;31m ")
read -p "[Pulse ENTER para volver al menu principal] "
f_menu
}
###########################################################
f_sana() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[+]\e[0;37m Agregando los repositorios y actualizando sorces.list\e[0m"
echo -e "\e[0;31mEspere...\e[0m" ; sleep 5
echo '#KALI LINUX SANA(2.0)' >> /etc/apt/sources.list  
echo 'deb http://old.kali.org/kali sana main non-free contrib' >> /etc/apt/sources.list
echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
echo '# deb-src http://old.kali.org/kali sana main non-free contrib' >> /etc/apt/sources.list
sudo apt update
echo -e "\e[0;31m[+]\e[0;32m Repsitorios agregados y actualizados correctamente.."
echo -e "\e[0;37m " $(echo -e "\e[0;31m ")
read -p "[Pulse ENTER para volver al menu principal] "
f_menu
}
############################################################
f_rolling() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[+]\e[0;37m Agregando los repositorios y actualizando sorces.list\e[0m"
echo -e "\e[0;31mEspere...\e[0m" ; sleep 5
echo '#KALI LINUX ROLLING' >> /etc/apt/sources.list  
echo 'deb http://http.kali.org/kali kali-rolling main contrib non-free' >> /etc/apt/sources.list
echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
echo '# deb-src http://http.kali.org/kali kali-rolling main contrib non-free' >> /etc/apt/sources.list
sudo apt update
echo -e "\e[0;31m[+]\e[0;32m Repsitorios agregados y actualizados correctamente.."
echo -e "\e[0;37m " $(echo -e "\e[0;31m ")
read -p "[Pulse ENTER para volver al menu principal] "
f_menu
}
############################################################
f_error() {
echo
echo -e "\e[0;31m<**********************>\e[0m"
echo -e "\e[0;31m<*******>>ERROR<<******>\e[0m"
echo -e "\e[0;31m<**********************>\e[0m" ; sleep 2
}
#
############################################################
f_salir() {
echo
echo -e "\e[0;31m[+]\e[0;37m Saliendo del script...\e[0m"
sleep 3
clear
reset
exit 0
}
############################################################
f_kali_moto() {
clear
echo
f_banner
echo -e "\e[0;31m[+]\e[0;37m Se instalara el repositorio de kali linux moto a su distribucion\e[0;31m "$(uname -n)
echo -e "\e[0;31mEspere...\e[0m"; sleep 5
sudo  apt-key adv --keyserver pgp.mit.edu --recv-keys ED444FF07D8D0BF6
sudo echo '#KALI LINUX MOTO (1.0)' >> /etc/apt/sources.list  
sudo echo 'deb http://old.kali.org/kali moto main non-free contrib' >> /etc/apt/sources.list
sudo echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
sudo echo '# deb-src http://old.kali.org/kali moto main non-free contrib' >> /etc/apt/sources.list
sudo apt update 
echo -e "\e[0;31m[+]\e[0;32m Instalado y actualizado correctamente..\e[0m"
echo -e "\e[0;37m " $(echo -e "\e[0;31m ")
read -p "[Pulse ENTER para volver al menu principal] "
f_menu
}
############################################################
f_instalar_kali() {
clear
echo
f_banner
echo -e "\e[0;31m[+]\e[0;37m Instalando repositorios kali linux rolling.....\e[0m"
sudo  apt-key adv --keyserver pgp.mit.edu --recv-keys ED444FF07D8D0BF6
echo '#KALI LINUX ROLLING' >> /etc/apt/sources.list  
echo 'deb http://http.kali.org/kali kali-rolling main contrib non-free' >> /etc/apt/sources.list
echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
echo '# deb-src http://http.kali.org/kali kali-rolling main contrib non-free' >> /etc/apt/sources.list
echo -e "\e[0;31m[+]\e[0;37m Actualizando nuevos repositorios...\e[0m"
echo -e "\e[0;36m "
sudo apt-get  update
echo -e "\e[0;31m[+]\e[0;37m Instalando kali linux\e[0;32m full\e[0;37m en su distribucion :\e[0m" $(uname -n)
echo -e "\e[0;36m "
sudo apt-get install kali-linux-full
echo -e "\e[0;31m[+]\e[0;37m Kali linux full se ha instalado correctamente.\e[0m"
echo -e "\e[0;31m "
read -p "[PULSE ENTER PARA VOLVER AL MENU PRINCIPAL]"
f_menu
}
############################################################
f_kali_sana() {
clear
echo
f_banner
echo -e "\e[0;31m[+]\e[0;37m Se instalara el repositorio de kali linux moto a su distribucion\e[0;31m "$(uname -n)
echo -e "\e[0;31mEspere...\e[0m"; sleep 5
sudo  apt-key adv --keyserver pgp.mit.edu --recv-keys ED444FF07D8D0BF6
echo '#KALI LINUX SANA(2.0)' >> /etc/apt/sources.list  
echo 'deb http://old.kali.org/kali sana main non-free contrib' >> /etc/apt/sources.list
echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
echo '# deb-src http://old.kali.org/kali sana main non-free contrib' >> /etc/apt/sources.list
sudo apt update 
echo -e "\e[0;31m[+]\e[0;32m Instalado y actualizado correctamente..\e[0m"
echo -e "\e[0;37m " $(echo -e "\e[0;31m ")
read -p "[Pulse ENTER para volver al menu principal] "
f_menu
}
############################################################
f_kali_rolling() {
clear
echo
f_banner
echo -e "\e[0;31m[+]\e[0;37m Se instalara el repositorio de kali linux moto a su distribucion\e[0;31m "$(uname -n)
echo -e "\e[0;31mEspere...\e[0m"; sleep 5
sudo  apt-key adv --keyserver pgp.mit.edu --recv-keys ED444FF07D8D0BF6
echo '#KALI LINUX ROLLING' >> /etc/apt/sources.list  
echo 'deb http://http.kali.org/kali kali-rolling main contrib non-free' >> /etc/apt/sources.list
echo '# For source package access, uncomment the following line' >> /etc/apt/sources.list
echo '# deb-src http://http.kali.org/kali kali-rolling main contrib non-free' >> /etc/apt/sources.list
sudo apt update 
echo -e "\e[0;31m[+]\e[0;32m Instalado y actualizado correctamente..\e[0m"
echo -e "\e[0;37m " $(echo -e "\e[0;31m ")
read -p "[Pulse ENTER para volver al menu principal] "
f_menu
}
############################################################
f_instalar_repos() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[+]\e[0;37m Repositorios disponibles para instalar.\e[0m"
echo "---------------------------------------------"
echo -e "\e[0;31m[1]\e[0;37m kali linux Moto.\e[0m"
echo -e "\e[0;31m[2]\e[0;37m kali linux Sana.\e[0m"
echo -e "\e[0;31m[3]\e[0;37m kali linux Rolling.\e[0m"
echo -e "\e[0;31m[4]\e[0;37m Menu principal.\e[0m"
echo -e "\e[0;31m[5]\e[0;37m Salir.\e[0m"
echo -e "\e[0;37m "
	read -p "Opcion> " OPCION2
case $OPCION2 in
	1) f_kali_moto
	;;
	2) f_kali_sana
	;;
	3) f_kali_rolling
	;;
	4) f_menu
	;;
	5) f_salir
	;;
	*) f_error
esac
}
############################################################
				f_agregar_repos() {
				clear
				echo
				f_banner
				echo
				echo -e "\e[0;31m[+]\e[0;37m Repositorios disponibles para agregar.\e[0m"
				echo "---------------------------------------------"
				echo -e "\e[0;31m[1]\e[0;37m Moto.\e[0m"
				echo -e "\e[0;31m[2]\e[0;37m Sana.\e[0m"
				echo -e "\e[0;31m[3]\e[0;37m Rolling.\e[0m"
				echo -e "\e[0;31m[4]\e[0;37m Menu principal.\e[0m"
				echo -e "\e[0;31m[5]\e[0;37m Salir.\e[0m"
				echo -e "\e[0;37m "
				read -p "Opcion> " OPCION
				case $OPCION in
					1) f_moto
					;;
					2) f_sana
					;;
					3) f_rolling
					;;
					4) f_menu
					;;
					5) f_salir
					;;
					*) f_error
				esac
}
########################################################
f_menu() {
clear
echo
f_banner
echo
echo -e "\e[0;31m[Menu principal del script]\e[0;37m Tome usted la decision.\e[0m"
echo "---------------------------------------------------"
echo -e "\e[0;31m[1]\e[0;37m Listar repositorios en pantalla.\e[0m"
echo -e "\e[0;31m[2]\e[0;37m Instalar repositorios \e[0;32m(solo si NO esta en kali linux)\e[0m"
echo -e "\e[0;31m[3]\e[0;37m Actualizar repositorios.\e[0m"
echo -e "\e[0;31m[4]\e[0;37m Lanzar Auto-Apt.\e[0;32m(solo SI esta instalado.)\e[0m"
echo -e "\e[0;31m[5]\e[0;37m Editar sources.list\e[0m"
echo -e "\e[0;31m[6]\e[0;37m Agregar repositorios a sources.list\e[0;32m (Solo SI esta en kali linux)\e[0m"
echo -e "\e[0;31m[7]\e[0;37m Instalar \e[0;31mkali linux full\e[0;37m en mi distribucion favorita.\e[0;32m (Solo si NO esta en kali linux)\e[0m"
echo -e "\e[0;31m[8]\e[0;37m Salir.\e[0m"
echo -e "\e[0;37m "
read -p "Opcion> " OPCION1

	case $OPCION1 in
		1) f_ver_repositorios
		;;
		2) f_instalar_repos
		;;
		3) f_actualizar
		;;
		4) f_auto_apt
		;;
		5) f_editar
		;;
		6) f_agregar_repos
		;;
		7) f_instalar_kali
		;;
		8) f_salir
		;;
		*) f_error
		;;
	esac
}
########################################################
while true; do f_menu; done

