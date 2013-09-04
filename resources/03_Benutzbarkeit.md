
# Benutzbarkeit

## Was bedeutet Benutzbarkeit?

Aufwand, der zur Benutzung erforderlich ist, und individuelle Beurteilung der Benutzung durch eine festgelegte oder vorausgesetzte Benutzer-gruppe. Hierunter fällt auch der Bereich Softwareergonomie.

Zu Benutzbarkeit gehören nach DIN/ISO 9126 folgende Teilmerkmale:

* _Verständlichkeit_: Aufwand für den Benutzer, das Konzept und die Anwendung zu verstehen.
* _Erlernbarkeit_: Aufwand für den Benutzer, die Anwendung zu erlernen (z.B. Bedienung, Ein-, Ausgabe)
* _Bedienbarkeit_: Aufwand für den Benutzer, die Anwendung zu bedienen.




## Szenarien für Benutzbarkeit
#### Szenario: Das interaktive Testwerkzeug muss einfach benutzbar sein. Tester (für den Benutzer-Akzeptanztest) müssen innerhalb von zwei Stunden die Bedienung erlernen können.  

Geschäftsziel(e):
Produktive und schnelle Akzeptanztests, schnelle Durchläufe 
Auslöser
Ein BA-Tester testet mit dem Testwerkzeug ein neues Release der Software.
Reaktion:
Der Tester kann das Testwerkzeug vollständig bedienen.
Zielwert:
Benötigt dafür weniger als zwei Stunden Einarbeitung.

#### Szenario: Endanwender / Endbenutzer können identische Tastaturkürzel ("keyboard shortcuts") in allen, unabhängig voneinander entwickelten, Modulen des Systems verwenden. 

Geschäftsziel(e):
Konsistente Benutzerführung ("User experience") im gesamten Produkt
Auslöser
Benutzer möchte Tastatur zur Navigation innerhalb des Systems verwenden
Reaktion:
Benutzer kann die gleichen Funktionen wie bei der Benutzung der Maus ausführen.
Zielwert:
Die Tastaturkürzel sind einheitlich vergeben. Bei Verwendung der Tastatur können sämtliche Funktionen schneller oder mindestens genauso schnell wie bei Nutzung der Maus verwendet werden.


#### Szenario: Benutzer soll auch Informationen, die nicht im Zusammenhang mit der aktuellen Bildschirmmaske stehen, schnell erfassen können. 
Qualitätsziele: Benutzbarkeit, Effizienz 
Geschäftsziel(e):
Einfache Benutzbarkeit, einfache Navigierbarkeit innerhalb des Systems
Auslöser:
Der Benutzer arbeitet mit dem System. Während der Bearbeitung einer Bildschirmmaske möchte er zu einem gänzlich anderen Thema Informationen erfassen oder bearbeiten.
Reaktion:
Der Benutzer kann einfach zu dem gewünschten Thema navigieren und nach dessen Bearbeitung einfach zum aktuellen Thema zurückkehren.
Zielwert:
Navigation zum gewünschten Thema erfolgt in weniger als 10 Sekunden, die Rückkehr zum aktuellen Thema erfolgt mit nur einem Knopfdruck / Mausklick.


#### Szenario: Benutzer werden grundsätzlich auf inkonsistente oder fehlerhafte Eingaben hingewiesen. 

Geschäftsziel(e):
Konsistenz bei Benutzereingaben
Auslöser / Stimulus:
Benutzer gibt Daten ein.
Reaktion:
Das System nimmt korrekte Eingabedaten an, weist inkonsistente oder fehlerhafte Eingabedaten zurück.
Zielwert:
Im Falle inkonsistenter oder fehlerhafter Eingabedaten gibt das System eine passende Meldung, die den Fehler oder die Inkonsistenz eindeutig und einfach aufzeigt.

#### Szenario: Falls ein Benutzer die pdf-Generierung des XY-Reports unterbricht, hält das System diese Generierung an und übergibt die Kontrolle innerhalb von 15 Sekunden wieder an die Benutzeroberfläche. 

Geschäftsziel(e):
Verbessere die Benutzbarkeit der pdf-Generierung
Auslöser / Stimulus:
Benutzer möchte die pdf-Generierung des XY-Reports unterbrechen (etwa aufgrund vorheriger Fehleingaben oder sonstiger Gründe) und klickt den "Abbrechen"-Button
Reaktion:
Das System unterbricht die Generierung, speichert den bisherigen Generierungszustand (für eventuelle Fortsetzungen) und übergibt die Kontrolle an die Benutzeroberfläche. 
Zielwert:
Benutzer erhält Kontrolle über das UI innerhalb von 15 Sekunden (d.h. In spätestens 15 Sekunden haben alle beteiligten Generierungsprozesse den Abbrechen-Befehl erfolgreich quittiert).
Bemerkung: Die Generierung dieses Reports läuft in mehreren parallelen Threads (oder Prozessen), eventuell sogar auf mehreren unterschiedlichen Prozessoren oder (virtuellen) Maschinen. Die Unterbrechung muss synchron und konsistent über alle diese Ausführungsinstanzen erfolgen.

#### Szenario: Falls eine Fehlersituation auftritt, wird dies dem Benutzer in aussagekräftigen Meldungen angezeigt. Das System stürzt bei Ausnahmesituationen (Speicherüberlauf, Hardwarefehler) nicht ab, sondern fährt höchstens kontrolliert heruntre.

Geschäftsziel(e):
Verbessere die Benutzbarkeit (und gefühlte Zuverlässigkeit). Ermögliche Benutzern, zu Fehlern führende Kombinationen von Eingabedaten zu korrigieren, ohne dass das System abstürzt.
Auslöser / Stimulus:
Ein Fehler / Ausnahmesituation in der Infrastruktur tritt auf (Speicherüberlauf, Out-of-Memory, Hardwarefehler).
Reaktion:
Das System erkennt den Fehler, meldet (soweit möglich) an den Benutzer und fährt kontrolliert herunter. 
Zielwert:
Fehlererkennung erfolgt innrehalb von 15 Sekunden, Meldung an Benutzer (sofern noch möglich) innerhalb von 1 Sekunde, herunterfahren innerhalb von 15 Sekunden. 

#### Szenario: Das System zeigt den Fortschritt der lange laufenden XY-Konvertierungsprozesse in der grafischen Oberfläche dem Benutzer an. 
Anmerkung: Diese XY-Konvertierung dauert 1-18 Stunden.
Geschäftsziel(e):
Fortschrittsüberwachung, Benutzerfreundlichkeit
Auslöser / Stimulus:
Benutzer möchte über Fortschritt der lang laufenden Berechnungen/Prozesse informiert werden.
Reaktion:
Das System zeigt die Anzahl der bisher verarbeiteten Datensätze, das verarbeitete Datenvolumen in Megabyte sowie den geschätzten verbleibenden Restaufwand an der GUI an. 
Zielwert:
Die Aktualisierung dieser Informationen erfolgt mindestens alle 60 Sekunden - höchstens alle 5 Sekunden.

#### Szenario: Das System soll den Auflagen und Vorschlägen der Microsoft Windows User Experience Guidelines für Windows-8 entsprechen. 

Geschäftsziel(e):
Einheitliches, dem Windows-8 Look-and-Feel entsprechendes Aussehen und Verhalten.
Auslöser / Stimulus:
Die Benutzeroberfläche und interaktiven Komponenten des Systems sollen neu gestaltet und implementiert werden.
Reaktion:

Zielwert:
Ein fachkundiger Auditor testiert die Übereinstimmung mit o.g. Guidelines ohne Einschränkung.

#### Szenario: Sämtliche Benutzerinteraktion und -meldungen im System sind als GUI implementiert. 

Geschäftsziel(e):
Erhöhe die Akzeptanz und Produktivität der Arbeit mit dem System.
Auslöser / Stimulus:
Alle Anforderungen an das System.
Reaktion:

Zielwert:
Das System erfordert keine Benutzerinteraktion außerhalb der grafischen Oberfläche.
