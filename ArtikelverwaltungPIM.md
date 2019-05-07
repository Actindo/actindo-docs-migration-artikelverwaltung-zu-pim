#Datenumzug mit dem Migrationsassistenten
###- Verschiebung der Daten aus der Artikelverwaltung in das PIM

[toc]

## 1. Hintergrund

Dieser Leitfaden für den Datenumzug richtet sich an Kunden, die Ihre Produktinformationen bislang in der Artikelverwaltung gespeichert haben und einen Umstieg Ihrer Daten auf das Actindo PIM Modul planen.

![Artikelverwaltung zu PIM - Page 6](/assets/Artikelverwaltung%20zu%20PIM%20-%20Page%206.jpeg)

###1.1 Begriffserklärung

Um Sie vorab hinsichtlich der verwendeten Begrifflichkeiten abzuholen, hier ein kurzer Einblick in die Bezeichnung und Funktion des neuen Moduls „PIM“, sowie des Migrationsassistenten, welches als Teilbereich des UCS-Sync fungiert.

Das ***Actindo PIM***, kurz für Product Information Management, führt die gesamten Produktinformationen zusammen, damit diese dann intern als auch extern genutzt werden können. Dabei ersetzt das PIM die bisherige Artikelverwaltung, in welcher Sie bisher Ihre Produktinformationen gepflegt und gespeichert haben.

Um diesen Datenumzug von der Artikelverwaltung (altes Modul) auf das PIM (neues Modul) durchzuführen, wird ein Migrationsassistent benötigt.

Der ***Migrationsassistent*** holt während des gesamten Prozesses die zu migrierenden Daten aus dem alten Modul, passt diese an und gibt sie dann an das neue Modul aus. Danach sorgt der Migrationsassistent dafür, dass bis zum vollständigen Ablegen der RetailSuite, die im PIM stattfindenden Arbeitsprozesse, automatisiert in der RetailSuite aktualisiert werden.

Der Migrationsassistent ist ein Teilbereich des ***UCS-Sync***. Der UCS-Sync Ist eine Schnittstelle zwischen alten und neuen Modulen, die die Kommunikation dieser ermöglicht.

Die ***Unified Commerce Suite*** (Abk. UCS), ist eine neue Softwaregeneration basierend auf der Actindo Core1. Sie setzt sich durch ein Set von verschiedenen Actindo Modulen zusammen. Dadurch ergibt sich ein vollumfängliches ERP, um Ihren gesamten Handel abzubilden.

Die ***Actindo Core1*** beschreibt das Betriebssystem auf dem das ERP – in unserem Fall die UCS und andere Entwicklungen sowie Applikationen – betrieben werden kann.

###1.2 Die Ziele des Datenumzugs

Mit der Migration Ihrer Artikeldaten auf das neue Modul, wird der Grundstein einer vollständigen UCS-Migration gesetzt. Die Vorteile einer sukzessiven Einführung zeigen sich vor allem in der einfachen Umstellung für den Anwender, da eine nicht überfordernde Schritt-für-Schritt Umstellung erfolgt.

Weitere Migrationsziele, die sich für Sie daraus ergeben, sind unter anderem die flexible und effiziente Datenpflege, die sich aus der zentralen Speicherung und Verwaltung sämtlicher Produktinformationen ergibt. Dabei ist nur ein einmaliges Pflegen der Datenfelder notwendig und die Übertragung dieser in die jeweiligen Kanäle generiert sich automatisch.

Vor allem sollen aber die alten Workflows, in denen Prozesse in verschiedenen Richtungen ausgeführt wurden, durch einheitliche Datenströme ersetzt werden. Unter anderem fallen darunter die Arbeitsprozesse zwischen dem Multimarkets Modul, den Marktplätzen und dem Modul Fakturierung. 

##2. Vor dem Datenumzug

Sobald Sie das PIM und den RS-Sync installiert haben, können Sie diese Daten-Migration durchführen.

###2.1 Ist und Soll-Zustand

**Bisher** gibt die Artikelverwaltung die Artikel an das POS Light und die Artikeldaten an das Modul Multimarkets ab. Das Multimarkets Modul gibt dann die Bestellungen, die es aus den Marktplätzen erhalten hat an die Fakturierung ab. Dieser hat hingegen die Verkäufe durch das POS Light Modul erhalten. Im Anschluss sendet die Fakturierung den aktuellen Status an das Multimarkets, welches diesen dann an die Marktplätze weiterleitet.

![IST Zustand](/assets/IST%20Zustand.jpeg)

**Jetzt** soll das PIM die Artikeldaten an das Modul Channels senden, welches die Artikel an das Venduo POS weiterleitet, um im Gegenzug die Verkäufe zu erhalten. Das Channels Modul kann so immer den aktuellsten Status an die Marktplätze übermitteln und erhält im Gegenzug die Bestellungen.

Damit die neuen Module PIM und Channels dabei mit dem alten Modul Fakturierung kommunizieren können, findet ein UCS-Sync zwischen diesen Modulen statt.

![SOLL Zustand](/assets/SOLL%20Zustand.jpeg)

###2.2 Der Ablauf des Datenumzugs

Damit der neue Prozessablauf integriert werden kann, müssen zuerst die Daten aus der Artikelverwaltung in das PIM eingespielt werden. Hierfür wird der Migrationsassistent, der als Teil des UCS-Sync agiert, in Betrieb genommen.

![Vorgehensweise](/assets/Vorgehensweise.jpeg)

##3. Der Auftrag zum Datenumzug

Sobald Sie Ihre Produktdaten umziehen wollen, beachten Sie folgende Vorgehensweise:

***Import starten***

Vorgehensweise:
* 1. Im Hauptmenü (links) auf Artikelverwaltung klicken.
* 2. Nun können Sie für Ihren Vorgang Import Starten auswählen.

![Datenimport Starten](/assets/Datenimport%20Starten.png)

Nachdem Sie diesen Befehl gegeben haben, findet von unserer Seite aus Ihre Datenmigration statt. Dafür verwenden wir einen von uns entwickelten Migrations-Assistenten, der Ihre Daten sortiert und vollständig in das neue Modul überträgt.

Der Migrationsassistent zeigt Ihnen beim Datenimport den Status Ihrer Migration an.


Es werden ausschließlich die Daten aus dem Modul „Artikelverwaltung“ übertragen. Dabei holt der Migrations-Assistent alle Produktinformationen aus dem alten Modul ab und gibt diese angepasst in das neue Modul ab. Dieser Vorgang kann je nach der Menge Ihrer Daten zwischen wenigen Stunden bis zu einem Tag dauern.

* Währenddessen können Sie alle weiteren Module (ausschließlich der Artikelverwaltung) ohne Einschränkungen verwenden.
* Nach Abschluss der Datenübermittlung, können Sie direkt mit dem PIM und dessen neuen Daten weiterarbeiten.
* Bei der Verwendung und Erweiterung der neuen Daten im PIM, werden diese bis zu Ihrer vollständigen UCS-Migration weiterhin in der Artikelverwaltung aktualisiert, um Datenverluste auszuschließen.
* Da das Multimarkets-Modul seine Daten aus dem Artikelverwaltungs-Modul bezieht, überträgt das PIM weiter alle Daten in die Artikelverwaltung.

##4. Nach dem Datenumzug

###4.1 Umgezogene Funktionen

* Alle Marktplätze, die bisher über das Multimarkets-Modul angebunden waren, werden jetzt über das Channels Modul angebunden.
* Das Channels Modul bezieht seine Daten direkt aus dem PIM
* Jetzt fügen Sie Ihre zukünftigen Artikeldaten direkt in das PIM ein.
