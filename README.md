<img width="196" alt="image" src="https://github.com/MuhammadHasoun/SpheroBolts/assets/159450804/07ffc8ca-9860-48fb-9427-e1d09edde650"># SpheroBolts
Code waarmee mensen verbinding kunnen maken met Sphero Bolts om ze te besturen met python.

# Benodigdheden
1. pip install bleak
2. pip install colorama

# Belangrijk!
Deze code is niet officieel van Sphero; dit hebben mijn teamgenoten en ik samen ontwikkeld.
We hebben code van een vorig project gebruikt en hebben het duidelijker gemaakt, zodat iedereen de code begrijpt.

*Zorg ervoor dat spherov3.py en sphero_constructors.py zich in dezelfde map bevinden waar je project wordt gemaakt.

# Functies
In onze spherov3-code hebben we twee klassen:
1.Scanner
* Deze klasse bevat een scan-methode. Wanneer de methode wordt aangeroepen, krijg je alle bolts te zien.

* De scan-methode bevat ook een debug-argument met twee opties die je kunt gebruiken:
  debug = "bolts" OF debug = "readable" -- dit geeft de MAC-adressen van alle beschikbare bolts in een lijst;
  Geen Debug - dit print alle bolts met namen en mac adres in de opdrachtregel.
  
* Dit scant de omgeving voor beschikbare bolts en laat zien welke bolts je kunt verbinden.
  
2.spherov3_connector
* Deze klasse bevat 4 functies:
  1. .connect - Dit maakt verbinding met het MAC-adres van de bolt dat je hebt opgegeven. Argumenten(Mac_address)
  2. .roll - Nadat je verbinding is gelukt, kun je met de 'roll'-functie je bolt besturen. Deze functie vereist twee verplichte argumenten (snelheid, richting), waarbij de snelheid aangeeft hoe snel de bolt moet rollen en de richting aangeeft waarheen de bolt moet rollen. Bijvoorbeeld: (50, 180) betekent dat de bolt met een snelheid van 50 naar 180 graden rolt, dus naar voren.
  3. .rest_yaw - Dit brengt de bolt terug naar de standaardpositie. -Geen Argumenten
  4. .disconnect - Sluit de verbinding met de bolt af. -Geen Argumenten


# Voorbeeld:
<img width="196" alt="image" src="https://github.com/MuhammadHasoun/SpheroBolts/assets/159450804/ac3180ba-fc93-4f43-a9cf-663e73298a74">

     







