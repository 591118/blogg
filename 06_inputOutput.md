---
title: 06_Input_Output
layout: home
---

## Input / Output

RESULTATET:


![GIF](assets/video.gif)

Jeg måler tempraturen gjennom Adafruit feather nrf52840 sense, som inneholder en tempratursensor. 
Lysene vil bevege seg når tempraturen er over 27 grader, som vist på bildet.

Derfor måler jeg tempratur, men når prosjetet er ferdig, vil jeg slå lysene på ved tid.
Dette ble dermed et litt lettere eksempel, enn det jeg vil bruke i den ferdige prototypen.

Det jeg vil måle i den ferdige prototypen er:
    - Tid
    - Tempratur
    - Luftfuktighet (humidity)

    For å evaluere søvnkvalitet.

Jeg måler hvert 0,5 sekund, for å få en presis start/stopp av lysene.
For det ferdig prototypen trenger jeg etter aktivert "natt" (mellom kl 23-06) trenger jeg ikke så ofte registeringer. Kanskje hver halvtime/time.
Muligens 1 gang i minuttet, hvis tempratur & luftfuktighet er viktig for søvnkaliteten.


Dataene i tempratur & lys ble som forventet. Bortsett fra at lyset var på etter at tempraturen var mindre enn 27 grader. Lyset stoppet, mens jeg trodde det skulle slå seg av. Har derimot funnet "feilen" i koden.

Det står på https://learn.adafruit.com/adafruit-dotstar-leds/dotstar-strips at jeg trenger 43 watt, 8,6 Amps på 5 V, for 144 LED på full styrke. 