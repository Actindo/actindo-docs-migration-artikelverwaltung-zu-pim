[toc]

# PIM

##Das Actindo PIM

Das ***Actindo PIM*** (kurz für Product Information Management) ist die zentrale Sammelstelle der Produktinformationen über alle Plattformen hinweg.

Hier werden alle Informationen Ihrer Produkte (mit eingeschlossen Marketingtexte sowie Informationen aus dem ERP-System) gesammelt um dann Online, in Print und auf dem Verkaufsetikett zu erscheinen.

![PIM - Page 2](pim1.jpg)

***Wie passiert das?***

*(technisch)*
Durch eine Software-Lösung werden Workflows abgebildet, die die zentrale Speicherung und Verwaltung sämtlicher Produktinformationen ermöglichen und die automatisierte Übertragung dieser in die jeweiligen Kanäle generiert. Da diese Daten medienneutral verwaltet werden, geschieht die Datenpflege und -erfassung effizient und mit wenig Aufwand.

Durch die Erfassung eines bestimmen DataHub-Datenmodells bestimmen Sie vorab Attribute und Felder, die dann auf jeden Datensatz übertragen werden und sich immer gleichen.

***Warum brauchen Sie es?***

Um sich abzuheben, müssen Sie mit hochwertigem Content überzeugen. Vom Online-Shop bis hin zum POS (Point of Sale) muss Ihre Produktinformation up-to-date und vollständig sein. Nur so erhöhen Sie Ihren Servicegrad - um wiederum die Kundenzufriedenheit zu garantieren - um dann im Idealfall einen Geschäftsabschluss zu erreichen. Mithilfe des Actindo PIMs gehen Ihnen keine wichtigen Daten verloren und jeder Mitarbeiter greift auf die gleichen Informationen zurück.

![PIM - Page 3](pim2.jpg)

***Ab wann ist ein PIM sinnvoll?***

* Wenn Sie über ein umfangreiches Sortiment verfügen.

* Wenn Sie mehrere Vertriebskanäle verwenden (Omnichannel Commerce).

* Wenn Sie Zusatzdokumente verwalten möchten (Bilder, Audio-Dateien, Videos etc.)

* Wenn Sie regelmäßig Ihre Produktinformationen anpassen.

* Wenn Sie internationalen Vertrieb betreiben.

* Wenn Sie kürzere Verkaufswege wünschen (‚Time-To-Market‘) die aufgrund der Workflow-gestützen Datenpflege möglich wird.

##Actindo PIM Begriffserklärung

###1. Ausgabekanäle
Ein Ausgabekanal im Actindo PIM bezeichnet die ausgewählte Summe an gesammelten Produkten und deren Informationen, die über einen Ausgabekanal, exportiert werden sollen.

>Beispiel: E-Commerce Kanal für die Desktop-Webseite und ein weiterer Kanal für die Smartphone-Anwendung.


Ein Ausgabekanal ist gleichzusetzen mit einem Filter:
o	Kategorien-Auswahl (definiert die zu exportierende Produktauswahl)
o	Orts-Auswahl (definiert die benötigten Werte für den Kanal; (Beispiel: Beschränkung auf Produktinformationen auf einer Sprache, obwohl diese auch in anderen Sprachen vorzufinden sind)
o	Währungs-Auswahl (definiert welche Typ-Attribute benötigt werden; Beispiel: Preise in Euro und in Schweizer Franken aber nicht in Dollar)
o	Vollständigkeits-Auswahl (definiert welche Produktinformationen obligatorisch sind)
o	Produktfamilien-Auswahl (Beispiel: das Feld ‚Beschreibung‘ muss für den E-Commerce Kanal vorhanden sein aber für die mobile Version muss nur ‚Produktname‘ ausgefüllt sein)

###2. Vollständigkeit
Die Vollständigkeit bezeichnet im Actindo PIM, die totalen getätigten Produkteinträge. Sie gibt die Anzahl der befüllten Felder gegenüber der verfügbaren Felder an.

>Die Vollständigkeit eines Produkts ist dann gegeben, wenn alle Attribute, die nach seiner Familie als „erforderlich“ definiert sind und für einen Ausgabekanal Wert haben, befüllt sind.

###3. Attribute
Ein Attribut definiert eine bestimmte Eigenschaft. Ihr Wert kann für jeden Ausgabekanal und Sprache unterschiedlich sein. Mit erstellten und definierten Attributen werden Attribut-Sets gebildet, die dann verwendet werden können, um einer Entität eine Menge von Attributen zuzuweisen.

> [info] Ein Attribut kann immer nur **einer** Attribut-Gruppe zugeordnet werden.

> Beispiel: Das Attribut ‚Bild‘ kann nicht gleichzeitig in Artikeldaten und Bildern erscheinen.

**Attribut-Gruppen**
Attribute können auch in Gruppen und Untergruppen aufgeteilt werden. Dies soll die Attribute kategorisieren und Ordnung im Frontend schaffen.

**Basisdaten**
Ist eine Sammlung der Daten, die bei allen Attributgruppen angewendet werden und uniform sind.

###4. Produkttypen
Produkttypen meint die Einteilung von Produkten anhand festgelegter Merkmale. Je Produkttyp werden zusätzliche Attribute festgelegt, welche für den jeweiligen Produkttyp von belangen sind.

**PIM Basisset**
Ist eine Sammlung der Daten, die bei allen Artikeln angewendet werden und uniform sind.

###5. Kategorie
Im Actindo PIM dient die ‚Kategorie‘ zur Einteilung der Artikel für die internen- als auch / oder für die Ausgabekanäle.

Es können unendlich viele Produktkategorien erstellt werden. Zu finden sind diese dann im Produkt-Katalog.


###6. Variantensätze
Hier legt man die Artikelvarianten an. Artikelvarianten beschreiben die unterschiedlichen Merkmale eines Artikels. Variantensätze meint die Kollektion dieser. Mithilfe einer Variationsachse ist eine einzigartige Kombination der Attribut-Werte von Produkten möglich.

> Beispiel: Produkt: Mütze; Variantensatz mit folgenden Attributen: ‚Farbe‘ und ‚Größe‘; Variantenauslegung Farbe: Gelb, Rot, Grün; Variantenauslegung Größe: XS, S, L; usw. – Es kann sein, dass es nur eine Mütze mit den Attribut-Werten ‚Gelb‘ und der Attribut-Größe ‚S‘.

##Anzeige

| |  |
| :------| :------|
| SKU | 'Stock Keeping Unit' bezeichnet den Artikel im Lager durch eine zusätzliche Nummerierung für die eindieutige Identifizierung.|
| |  |
| Eigentümer App | Weißt auf die App-Zugehörigkeit hin. Da für ISV die Möglichkeit besteht eigene Apps zu entwickeln und im Actindo App-Store bereitzustellen, wird dementsprechend der Modul-Name angezeigt. |
| |  |
| ![read only](readonly.png) | *'Read only'* Attribute in diesem Reiter können lediglich eingesehen aber nicht geändert werden. Bei selbst angelegten Apps besteht die Möglichkeit einer Bearbeitung durch den Entwickler.|
| |  |
| Schlüssel | Dieser ist immer einzigartig und wird bei der Anlage durch den End-Nutzer vergeben. Der Schlüssel dient der Identifikation des Attribut-Sets. Relevant hat der Schlüssel vor allem für unsere Entwickler. Durch ihn lassen sich bei Problemen die gewünschten Produkte schneller identifizieren.|
| |  |
| ![aktiv](2aktiv.png) | *'Aktiv'* Reiter in diesem Zustand werden aktiv angewendet.|
| |  |
| ![inaktiv](1aktiv.png)| '*Inaktiv*' Reiter in diesem Zustand werden nicht angewendet.|


<div style="display: flex;">
    <img style="flex-basis: 50%; margin-right: 1em;" title="In Bearbeitung" src="In_Bearbeitung.svg"/>
    <div style="flex-basis: 50%;">
        <p>
            Diese Dokumentation befindet sich derzeit noch in Bearbeitung.
        </p>
    </div>
