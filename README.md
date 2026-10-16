![alt text](<2026-10-16 18_43_43-VirtualBoxVM.png>)
He utilitzat l’ordre cat /etc/group per mostrar els grups que hi ha creats al sistema Linux, amb els seus identificadors i els usuaris que en formen part.
![alt text](<2026-10-16 18_48_52-Oracle VirtualBox Gestor.png>)
Aquesta imatge mostra elsHe tornat a consultar el fitxer /etc/group per veure els grups del sistema i comprovar quins usuaris hi estan associats. 
![alt text](<2026-10-16 18_49_08-Oracle VirtualBox Gestor.png>)
He intentat consultar un fitxer de grups anomenat benvinguda.txt, però ha aparegut un error perquè el fitxer no existeix a la ruta indicada.
![alt text](<2026-10-16 18_49_39-Oracle VirtualBox Gestor.png>)
He creat la carpeta Documents dins del directori personal amb l'ordre mkdir -p ~/Documents.
![alt text](<2026-10-16 18_50_05-Oracle VirtualBox Gestor.png>)
He accedit al directori de configuració /etc/skel i he obert el fitxer .bashrc amb l'editor Nano per consultar-ne o modificar-ne la configuració.
![alt text](<2026-10-16 18_52_18-Oracle VirtualBox Gestor.png>)
He consultat el fitxer de configuració /etc/adduser.conf amb l'editor Nano. Aquest fitxer conté els paràmetres que s'utilitzen per crear nous usuaris.
![alt text](<2026-10-16 18_54_30-Oracle VirtualBox Gestor.png>)
He executat l'ordre sudo adduser prova1 per crear un usuari nou anomenat prova1, establint una contrasenya i configurant-ne les dades.
![alt text](<2026-10-16 18_54_44-Oracle VirtualBox Gestor.png>)
He comprovat el resultat de la creació de l'usuari prova1 i he consultat el contingut del directori per verificar els fitxers de configuració que s'hi han generat.
![alt text](<2026-10-16 18_55_27-Oracle VirtualBox Gestor.png>)
He creat l'usuari pau_dev amb l'ordre sudo adduser pau_dev, establint-ne una contrasenya i configurant les dades inicials.
![alt text](<2026-10-16 18_55_58-Oracle VirtualBox Gestor.png>)
He creat l'usuari laura_dev amb l'ordre sudo adduser laura_dev, assignant-li una contrasenya i configurant-ne les dades.
![alt text](<2026-10-16 18_56_59-Oracle VirtualBox Gestor.png>)
He intentat crear un grup anomenat devs, però el sistema ha indicat que el grup no existia en executar una ordre que el necessitava. Després he utilitzat sudo addgroup devs per crear-lo.
![alt text](<2026-10-16 18_58_24-Oracle VirtualBox Gestor.png>)
He modificat la informació dels usuaris amb ordres com usermod per assignar-los grups i configurar les seves dades, com ara el directori personal i l'intèrpret d'ordres.
![alt text](<2026-10-16 18_59_03-Oracle VirtualBox Gestor.png>)
He continuat modificant la configuració dels usuaris pau_dev, laura_dev i altres comptes, assignant-los grups i establint les opcions corresponents.
![alt text](<2026-10-16 18_59_15-Oracle VirtualBox Gestor.png>)
He consultat la informació dels usuaris amb l'ordre cat /etc/passwd. Aquest fitxer mostra els comptes existents, els seus identificadors, els directoris personals i els intèrprets d'ordres configurats.
![alt text](<2026-10-16 18_59_31-Oracle VirtualBox Gestor.png>)
He intentat consultar el fitxer /etc/shadow amb permisos d'administrador, però el sistema ha indicat que l'usuari pau_dev no forma part del grup d'usuaris autoritzats a utilitzar sudo.
![alt text](<2026-10-16 19_00_57-Oracle VirtualBox Gestor.png>)
He tornat a consultar els fitxers dels comptes d'usuari per comprovar la configuració dels diferents usuaris i els seus intèrprets d'ordres.
![alt text](<2026-10-16 19_01_17-Oracle VirtualBox Gestor.png>)
He intentat accedir al fitxer /etc/shadow amb l'ordre sudo cat /etc/shadow, però no ha estat possible perquè l'usuari no té permisos d'administrador.
![alt text](<2026-10-16 19_01_48-Oracle VirtualBox Gestor.png>)
He revisat el contingut del fitxer /etc/passwd per comprovar les dades dels usuaris creats i els intèrprets d'ordres que tenen assignats.
![alt text](<2026-10-16 19_02_09-Oracle VirtualBox Gestor.png>)
He tornat a provar d'accedir al fitxer /etc/shadow i he comprovat que el compte pau_dev continua sense tenir permisos per executar ordres amb sudo.
![alt text](<2026-10-16 19_02_26-Oracle VirtualBox Gestor.png>)
He revisat el fitxer /etc/passwd per verificar els comptes d'usuari i comprovar les seves dades de configuració.
![alt text](<2026-10-16 19_06_22-Greenshot.png>)
He repetit la consulta del fitxer /etc/shadow i he comprovat que l'usuari pau_dev no està autoritzat a executar l'ordre amb permisos d'administrador.
![alt text](<2026-10-16 19_07_46-.png>)
He tornat a consultar el fitxer /etc/passwd i he comprovat que els usuaris creats apareixen al sistema amb els seus directoris personals i els intèrprets d'ordres corresponents.
![alt text](<2026-10-16 19_08_44-Greenshot.png>)
He executat l'ordre sudo chsh -s /usr/bin/fish laura_dev per canviar l'intèrpret d'ordres predeterminat de l'usuari laura_dev a Fish.
![alt text](<2026-10-16 19_09_17-.png>)
He iniciat una sessió amb l'usuari laura_dev mitjançant l'ordre su - laura_dev. En iniciar sessió, s'ha mostrat el missatge de benvinguda de Fish.
![alt text](<2026-10-16 19_09_32-Greenshot.png>)
He comprovat que l'intèrpret d'ordres de laura_dev és Fish executant l'ordre echo $SHELL. El resultat /usr/bin/fish confirma que el canvi s'ha aplicat correctament.