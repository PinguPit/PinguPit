const rennfahrerData = {
    geschwindigkeit: 0, // in km/h
    herzfrequenz: 0, // in BPM
    rundenzeit: "00:00:00", // Zeitformat
};

const wetterData = {
    temperatur: 0, // in °C
    luftfeuchtigkeit: 0, // in %
    windgeschwindigkeit: 0, // in km/h
    wetterzustand: "sonnig", // sonnig, bewölkt, regnerisch
};

const streckeData = {
    name: "Hockenheimring",
    laenge: 4574, // in Metern
    breite: 0, // in Metern
    belag: "Asphalt",
    hoehe: 0, // Höhenunterschiede in Metern
    schnelleZonen: [], // Liste der schnellen Zonen
    langsameZonen: [], // Liste der langsamen Zonen
};

const reifenData = {
    abnutzung: 0, // in %
    temperatur: 0, // in °C
    druck: 0, // in PSI
};

const fahrzeugData = {
    kraftstoffmenge: 0, // in Litern
    oeltemperatur: 0, // in °C
    motortemperatur: 0, // in °C
};
function generiereRennfahrerData() {
    rennfahrerData.geschwindigkeit = Math.floor(Math.random() * (320 - 50 + 1)) + 50; // 50km/h bis 320km/h
    rennfahrerData.herzfrequenz = Math.floor(Math.random() * (180 - 60 + 1)) + 60; // 60BPM bis 180BPM
    // Rundenzeit kann komplexer sein, daher lassen wir es vorerst so
}

function generiereWetterData() {
    wetterData.temperatur = Math.floor(Math.random() * (35 - (-5) + 1)) - 5; // -5°C bis 35°C
    wetterData.luftfeuchtigkeit = Math.floor(Math.random() * 100); // 0% bis 100%
    wetterData.windgeschwindigkeit = Math.floor(Math.random() * 20); // 0km/h bis 20km/h
    const zustaende = ["sonnig", "bewölkt", "regnerisch"];
    wetterData.wetterzustand = zustaende[Math.floor(Math.random() * zustaende.length)];
}

// Ähnliche Funktionen können für `streckeData`, `reifenData` und `fahrzeugData` erstellt werden.


