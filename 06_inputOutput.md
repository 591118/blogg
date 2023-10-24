---
title: 06_Input_Output
layout: home
---

## Input / Output

RESULTATET:

Jeg måler tempraturen gjennom Adafruit feather nrf52840 sense.

Den inneholder en tempratursensor, for prosjektet ville jeg bruke at tid, slår på lyset for å kjøre.

Dette ble dermed et litt lettere eksempel, enn det jeg vil bruke i den ferdige prototypen.

Det jeg vil måle i den ferdige prototypen er:
    - Tempratur
    - Luftfoktighet


Jeg måler hvert 0,5 sekund, for å få en god nok samplingsdata i dette prosjektet.

For prosjektets vil det være avhenig av tiden.
Om natten vil det være tilstrekkelig med målinger 1 gang i minuttet, hvis tempratur & luftfuktighet er viktig.

Hvis ikke kan det være tilstrekkelig å måle en gang i timen om natten. Sjekke klokken, og sjekke hvert 30 minutt fra kl 6, og hvert 5 min fra kl 630.


Dataene i tempratur & lys ble som forventet. Bortsett fra at lyset var på etter at tempraturen var mindre enn 27 grader. Det var koden, som ikke slo av lyset.

Det står på https://learn.adafruit.com/adafruit-dotstar-leds/dotstar-strips at jeg trenger 43 watt, 8,6 Amps på 5 V, for 144 LED på full styrke. 