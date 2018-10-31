# Kursrom Panel

Dette prosjektet omhandler et front-end GUI system for å presentere et touch-vennlig grensesnitt til brukere av kursrom o.l. som har behov for å kunne enkelt endre VLAN som kurs-PCer er koblet i, uten å måtte ringe IT-support. 

Systemet henger sammen med back-end prosjektet Network Configuration Scheduler som utfører selve konfigurasjonen basert på templates som er lagret i forhold til interface-konfigurasjonen på Cisco-svitsjene i systemet.

Kommunikasjonen til back-end går gjennom Rabbit MQ som en strukturert melding med forespørsel om å endre rom "X" til sone "Y", hvor sone representerer navnet på et VLAN. I kommunal sektor er flersone-modellen utbredt med interne, sikre og offentlige soner separert i flere VLAN, og det er her systemet og benevnelsene stammer fra.

