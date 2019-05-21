# Vor dem Datenumzug

Sobald Sie das PIM und den RS-Sync installiert haben, können Sie diese Daten-Migration durchführen.

### 2.1 Ist und Soll-Zustand

**Bisher** gibt die Artikelverwaltung die Artikel an das POS Light und die Artikeldaten an das Modul Multimarkets ab. Das Multimarkets Modul gibt dann die Bestellungen, die es aus den Marktplätzen erhalten hat an die Fakturierung ab. Dieser hat hingegen die Verkäufe durch das POS Light Modul erhalten. Im Anschluss sendet die Fakturierung den aktuellen Status an das Multimarkets, welches diesen dann an die Marktplätze weiterleitet.

![PIMist](/assets/PIMist.jpeg)

**Jetzt** soll das PIM die Artikeldaten an das Modul Channels senden, welches die Artikel an das Venduo POS weiterleitet, um im Gegenzug die Verkäufe zu erhalten. Das Channels Modul kann so immer den aktuellsten Status an die Marktplätze übermitteln und erhält im Gegenzug die Bestellungen.

Damit die neuen Module PIM und Channels dabei mit dem alten Modul Fakturierung kommunizieren können, findet ein UCS-Sync zwischen diesen Modulen statt.

![PIMsoll](/assets/PIMsoll.jpeg)

### 2.2 Der Ablauf des Datenumzugs

Damit der neue Prozessablauf integriert werden kann, müssen zuerst die Daten aus der Artikelverwaltung in das PIM eingespielt werden. Hierfür wird der Migrationsassistent, der als Teil des UCS-Sync agiert, in Betrieb genommen.

![PIMexport](/assets/PIMexport.jpeg)
