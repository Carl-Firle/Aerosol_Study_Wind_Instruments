# Raw data and Emission Rates
Directory `Particle Counts` contains all raw data from the measurements. We included a translation table.
Row 8 lists aerosol spectrometers position (in cm) and particle size bin/category (Aerosol < 6.64 µm, Droplets > 6.64).
Columns bellow particle size bin list

The file `EmissionRates_wind instruments.xlsx` includes all emission rates with standard deviations.



https://www.wolfram.com/cdf-player/index.html 

https://www.wolfram.com/player/



Bei Umweltmessungen ist die Partikelkonzentration der Probenluft in der Regel so gering, dass sich im Messvolumen statistisch gesehen nur ein Partikel befindet. [S. 12]
Die Zählrate ergibt sich aus der Partikelanzahl dividiert durch die Volumenflussrate. [S. 13]
Durch die Erfassung der Partikelkonzentration und Partikelgröße kann somit die Größenverteilung der Aerosolpartikel bestimmt werden, die wiederum Grundlage ist für die Berechnung der Partikelmasse. [S. 13]
Bei der Darstellung der Massenverteilung wird unterhalb des eigentlichen Messbereichs ein zusätzlicher Kanal bis 0,23μm durch das Anpassen einer Lognormal-Verteilung extrapoliert. [S. 19]
Partikelkonzentration: 1 bis 2.000.000 Partikel/Liter [S. 19]
Probenvolumenstrom: 1,2 l/min [S. 19]
Messzeitintervalle: Wählbar: 6 sek. normal (für alle Kanäle) [S. 20]
Messmodi Staubmasse in [μg/m³] und Partikelkonzentration in [Partikel/Liter] [S. 41]
Ist das Gerät im Messmodus Partikelkonzentration, erscheint am rechten Rand die Einheit /l, also Partikel pro Liter. [S. 41]
Die Messwerte im Messmodus Counts werden in der Regel in der Einheit Partikel pro Liter dargestellt. Erfolgt die Messwertausgabe schneller als 1 Minute (Bsp. 6 Sekunden oder 3, 2 oder 1 Sekunde mit eingeschränktem Größenbereich), ist die Einheit Partikel pro 100ml. [S. 55]
Modell 1.109, Version 12.30 Messmodus Partikelanzahl (Counts): 6 sek Intervall: 31 Kanäle >0,25μm bis >32μm in P/100ml [S. 60]
In Carls Messdaten-Files „*_Dataset.xlsx “ sind alle Count-Werte in Partikel/Liter angegeben (d.h. mit 10 multip.)
Quantisierung der Count-Werte:
AS-50:	für dp > 2,53 µm 10 /l, für kleinere 50 /l
AS-150:	für dp > 2,00 µm 10 /l, für kleinere 50 /l
AS-300:	für dp > 2,00 µm 10 /l, für kleinere 50 /l


Tatsächlich registriert wurden bei jeder Einzelmessung nur einstellige Partikel-Anzahlen
kurze Messzeit (6s) → kleines Messvolumen (120 ml) bei
niedrigen Luftkonzentrationen (meist ≤ 200 P/l)
Die hohen Anzeigewerte kommen durch Multiplikation mit großen Umrechnungsfaktoren (10 bzw. 50) zustande
Die zufällige Fluktuation der Einzelmesswerte (Zählrauschen) ist maximal (single particle counting)
extrem niedriges Signal-Rauschverhältnis (SNR)
bei den meisten Einzelwerten < 1 → Messfähigkeit nicht gegeben
Zeitliche Signalverläufe (Transienten) sind erst erkennbar, wenn SNR durch Pooling erhöht wird
je 34 Einzelwerte werden zu einem Hilfswert gemittelt (= Integration über 204 s)
Zeitauflösung geht verloren (nur noch 6 Datenpunkte über 20 Minuten Dauer verfügbar)
Kurvenformen sind nicht mehr unterscheidbar (insbesondere Geraden vs. gekrümmte Transienten)
Es werden nur Geraden angepasst
Wegen des niedrigen SNR kann Validität der "well-mixed room air"-Annahme nicht überprüft werden
diese wird vorausgesetzt (weil sie in bisherigen Studien sehr gut funktioniert hat)
Aus der "well-mixed room air"-Annahme folgt, dass alle drei Spektrometer dieselbe Transiente anzeigen!
Die eine resultierende Gerade wird durch simultane Anpassung an alle drei Spektrometer-Transienten berechnet
Wegen Luftwechselrate Null (Qubus geschlossen) und Vernachlässigung von Partikelabsorption an Oberflächen
ist die Steigung der Geraden proportional zur Partikelfreisetzungsrate durch ProbandIn
So wird aus 606 Single-Particle-Counting-Werten eine einzige Emissionsrate in P/s
Deren Vertrauensbereich wird anhand der Anpassungsgüte geschätzt (mittels Bootstrap-Methode)
Emissionsrate bekommt Fehlerbalken (1σ), der Unsicherheit der Geradensteigung bei der Anpassung ausdrückt
![grafik](https://user-images.githubusercontent.com/92682699/140093794-285fae8b-8e69-4643-938d-c168bd46e765.png)

