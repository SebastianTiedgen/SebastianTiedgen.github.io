# Dokumentation
Erstellt von Sebastian Tiedgen als Einsendeaufgabe im Rahmen des Deep Learning Moduls der VFH.

## Nutzung

Es können 5,10,20,50 oder 100 Datenpunkte erstellt werden. Weiterhin kann die Anzahl der Layer, der Neuronen pro Layer
die Anzahl der Trainingsepochen spezifiziert werden. Mit den Buttons under fitting, best fitting und over fitting können
Preset-Einstellungen geladen werden. Nachdem die Parameter gewählt wurden, muss der Datensatz sowie das Modell erstellt werden.
Danach kann mit dem Training begonnen werden. Ist dies Abgeschlossen, kann mit dem Test-Button das Ergebnis der Prediction betrachtet werden.
Die Visualisierung erfolgt auf der rechten Seite. Weiterhin kann das aktuelle Model gespeichert und das zuletzt gespeicherte geladen werden,


## Verwendete Frameworks
TensorFlow.js: Tensorflow-Framework für Javascript, benutzt um ML zu realisieren.

tfjs-vis: Visualisierung von Model, Training und Prediction.

## Funktionsweise


Es werden die entsprechende Anzahl an Datenpunkte erstellt. Mit Math.Random werden zufällige X-Werte berechnet und dazu
die entsprechenden Y-Werte nach der Funktion y=(x+0.8)*(x-0.2)*(x-0.3)*(x-0.6).

Zusätzlich wird zu jedem Y ein Gaussisches Rauschen mit einer Varianz von 0.3 dazu addiert.

Die Punkte werden in einen Tensor umgewandelt und für das Training aufbereitet. Nach dem vollständigen Trainingsprozess
wird die Testfunktion ausgeführt, die eine Prediction über die genutzten Punkte trifft.




## Quellenangabe:
https://codelabs.developers.google.com/codelabs/tfjs-training-regression/index.html#0

https://www.tensorflow.org/js

https://stackoverflow.com/questions/25582882/javascript-math-random-normal-distribution-gaussian-bell-curve

https://riptutorial.com/javascript/example/8330/random--with-gaussian-distribution

https://www.tensorflow.org/js/guide/save_load

https://medium.com/@minions.k/underfit-and-overfit-explained-8161559b37db
