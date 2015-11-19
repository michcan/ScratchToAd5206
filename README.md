# ScratchToAd5206
Contient les outils pour faire communiquer scratch et le potentiomètre numérique AD5206.
Attention mode sauvage !!

Scratch communique avec arduino par le protocole Firmata. Il faut utiliser l'extension S2A dans Scratch à cette fin.
Firmata ne gère pas le protocole SPI, j'ai donc fais un lien en sauvage entre les sorties PWM et le SPI.
J'ai créer un version spéciale de Firmata (cf. CustomFirmata)
J'ai aussi modifier le fichier « scratch_command_handlers.py » de S2A.
Pour contrôler un canal du ad5206 il suffit donc de :
exporter CustomFirmata.ino sur l'arduino
lancer S2A(version modifiée) dans le terminal
utiliser le bloc « Ecrire sur la broche PWM … la valeur … »