# attiny85

L’écosystème Arduino sert de passerelle USB <-> Serial <-> ISP.

Voici les instructions pour envoyer du code et fabriquer son programmateur à partir d’un Arduino UNO.

# MATÉRIEL NÉCESSAIRE

1 Arduino UNO
1 attiny85
1 câble USB type A
6 câbles de prototypages Femelle / Mâle

# INSTALLATION ARDUINO IDE

Rendez-vous sur le site Arduino ![](https://arduino.cc) dans la section Software :
![Page d'Accueil Arduino](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_site_arduino.png?w=521&h=285&crop&ssl=1)

Télécharger la dernière version de l’IDE pour votre système d’exploitation :
![Page de Download](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_download.png?w=521&h=285&crop&ssl=1)

Vous pouvez choisir de faire une donation ou non juste avant de lancer le téléchargement :
![Pensez à faire une Donation](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_download.png?w=521&h=285&crop&ssl=1)

Installez l’Arduino IDE sur votre ordinateur. Pour les utilisateurs de Windows je vous recommande d’utiliser l’installeur qui contient le pilote USB pour les cartes Arduino.

# MISE EN PLACE DU PROGRAMMATEUR

Lancez l’Arduino IDE
![Image de Lancement](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_ide_lancement.png?w=521&h=386&crop&ssl=1)

Ouvrez ensuite l’exemple -> Arduino ISP :
![Arduino ISP](https://i2.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_isp.png?w=277&h=270&crop&ssl=1)

Connectez ensuite juste votre Arduino UNO à votre ordinateur à l’aide du cordon USB et uploadez le code :
![Type de Carte](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_ide_type_carte.png?w=521&h=177&crop&ssl=1)
![Port de Destination](https://i2.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_isp_port.png?w=521&h=136&crop&ssl=1)

Lancer l'upload Upload Terminé
C’est terminé, votre Arduino UNO est prêt pour envoyer du code sur votre attiny85.

# DEFINITION DE CARTE

Rendez-vous dans les préférences de l’Arduino IDE :
![Accès Préférences](https://i0.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_arduino_preferences_mod.png?w=521&h=369&crop&ssl=1)

Ajoutez l’adresse suivante :
```https://raw.githubusercontent.com/damellis/attiny/ide-1.6.x-boards-manager/package_damellis_attiny_index.json```

Validez en cliquant sur OK. Allez alors dans le gestionnaire de cartes :
![Gestionnaire de Cartes](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_gestionnaire_cartes.png?w=338&h=102&crop&ssl=1)

Gestionnaire de Cartes
![Ajout attiny](https://i2.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_ajout_attiny.png?w=179&h=102&crop&ssl=1)

**Une fois ces opérations faites, redémarrez l’Arduino IDE afin que tout soit bien pris en compte.**

Vous pouvez alors choisir les bons paramètres pour la carte :
![Type de Carte](https://i2.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_type_attiny.png?w=180&h=150&crop&ssl=1)

![Processeur](https://i0.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_processeur_85.png?w=337&h=150&crop&ssl=1)

![Vitesse d'Horloge](https://i2.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_crystal_8.png?w=521&h=217&crop&ssl=1)

![Port Programmateur](https://i1.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_port_arduino.png?w=356&h=97&crop&ssl=1)

![Type du Programmateur](https://i2.wp.com/anderson69s.com/wp-content/uploads/2017/08/TinyJewel85_programmateur_arduino_as_isp.png?w=161&h=97&crop&ssl=1)

# SOURCES & UPLOAD

Il ne reste plus qu’à connecter l’Arduino UNO avec la carte  :

ATTINY85 ===     Arduino Uno
+5V           ===        +5V
GND        ===        GND
PB0        ===    D11
PB1        ===    D12
PB2        ===    D13
RESET    ===    D10

ATTINY85  | Arduino Uno
------------ | -------------
+5V  | +5V
GND | GND
RESET | D10
PB0 | D11
PB1 | D12
PB2 | D13

Puis à envoyer le code sur l'attiny85 avec le bouton upload de l'Arduino IDE 🙂


