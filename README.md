addFNMTfirefox
==============

Script para añadir el certificado de la FNMT a Firefox en todas las cuentas de alumnos y profesores, partiendo del directorio home.
  
Lo primero que hace el script es instalar el paquete libnss3-utils para disponer del comando certutil, si no se encuentra instalado aún.  
  
He definido las siguientes variables en el script:  
certificateFile="FNMTClase2CA_FNMT_ES.pem"  
certificateName="FNMT Clase 2 CA - FNMT"  
certificateDB="cert8.db"  
homeDir="/home"  
depthDir=3  

Podéis modificarlas de acuerdo con vuestras necesidades.  
  
Por otra parte, definido una profundidad de búsqueda máxima y mínima de 3 del directorio del perfil del usuario porque nuestros usuarios se almacenan en /home/profesor/usuario y /home/alumnos/usuario. Si queréis utilizarlo con otra estructura de directorios, no tenéis más que modificar la profundidad (variable depthDir).

Esteban M. Navas Martín  
27/05/2014  
