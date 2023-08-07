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
