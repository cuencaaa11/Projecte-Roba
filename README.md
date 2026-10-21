### [WearSafe](https://github.com/cuencaaa11/Projecte-Roba)
WearSafe: resum del projecte

WearSafe sera una empresa que ven un rellotge intel·ligent amb GPS i un servei web. L’objectiu és que les famílies sàpiguen on és el seu fill i rebin un avís ràpid si hi ha algun perill. Nosaltres fem de l’empresa que dissenya i implanta tot el sistema
Com funciona

1. El rellotge. Porta GPS i es connecta per Wi-Fi a Internet. Cada 5 segons envia un senyal al servidor amb la posició, la bateria i l’hora. També té un botó SOS: si el nen el prem, l’avís arriba a la família a l’instant.

2. El servidor. És una màquina virtual al núvol (IaaS), accessible a wearsafe.cat amb connexió segura (HTTPS). Rep cada senyal, comprova que ve d’un rellotge autoritzat i el desa.

3. La base de dades. Guarda totes les posicions amb la seva data i hora, a més dels usuaris, les zones i les alertes. El client hi té accés a través de la web i pot consultar on ha estat el nen en un dia i una franja horària concretes. La web dibuixa el recorregut al mapa i mostra els llocs on s’ha aturat. L’historial es guarda un màxim d’un mes: les dades més antigues s’esborren soles. Així protegim la privacitat dels menors i només guardem el que cal.

4. La web. La família entra amb el seu usuari i contrasenya i hi troba:

    El mapa en directe amb la ubicació exacta del nen, la bateria i l’hora de l’última actualització.
    L’historial per dia i hora, amb el recorregut dibuixat.
    Les zones segures: es marca un lloc (casa, escola, parc) i un radi en metres o quilòmetres. Si el nen en surt, arriba una notificació.
    Les zones perilloses: la família pot marcar un riu, una carretera amb trànsit o unes obres, i rep un avís si el nen s’hi acosta.
    El llistat d’alertes i la gestió del compte.
    Una part de botiga :  on es vendran aquests rellotges de diferents colors i tamanys

5. Les alertes. Un programa del servidor revisa les dades de manera contínua. Avisa quan el nen surt d’una zona segura, entra en una zona perillosa o s’allunya massa de l’adult. També avisa si hi ha pluja, tempesta, vent fort o calor extrema a la seva posició, o si hi ha bateria baixa, SOS o el rellotge es queda sense connexió. Els avisos surten a la web i al mòbil de la família per Telegram.
Part de xarxa

Dissenyem i simulem a Packet Tracer la xarxa d’oficina de WearSafe, amb VLANs per separar administració, suport tècnic, servidors, invitats i proves de rellotges. Hi afegim DHCP, DNS, NAT i regles de seguretat (ACL). Al servidor real configurem DNS, HTTPS, firewall i còpies de seguretat.
