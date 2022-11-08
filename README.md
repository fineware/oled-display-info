# oled-display-info
File di esempio per l'integrazione dei display Oled da 0.96" in Home Assistant

In questo repository trovate i file necessari a compilare il file binario per utilizzare il modulo oled-display info all'ionterno di Home Assistant.

Ringraziamo i gestori del sito domhouse.it che ci sono stati di ispirazione per questa implementazione, e che hanno fornito una guida completa per la compilazione e la programmazione del dispositivo, consultabile a questo [link](https://domhouse.it/creare-un-display-informazioni-per-home-assistant-con-esphome/).

Il file .yaml fornito e' da considerarsi come una base per le personalizzazioni. Comprende quindi l'inizializzazione il WiFi, l'attivazione del metodo di upload media OTA e la visualizzazione delll'ora attuale e della temperatura ricavata da un sensore chiamato 'sensor.dati_temperature'. In assenza di tale sensore nel vostro Home Assistant non verra' visualizzata questa schemata.
Viene utilizzato il font 'BebasNeue-Regular.ttf' ricavato Google Fonts.

Una volta alimentato il device questo passera' in modalita' Access Point dopo circa 30 secondi, rendendo disponibile la rete 'display-info'. Collegandosi a questa rete WiFi da un PC, tablet o smartphone si potra' accedere alla pagina di selezione della propria rete wireless tramite l'indirizzo [192.168.4.1](http://192.168.4.1). Selezionando la propria rete domestica ed inserendo la password il device memorizzera' questi paramentri ed in futuro si colleghera' a questa rete.

Modificato il file .yaml e' possibile visualizzare qualsiasi parametro di Home Assistant, creare nuove pagine e scegliere font diversi.

