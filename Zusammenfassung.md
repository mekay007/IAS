
# Java Programme
## Übersetzung
1. Wie werden Java Programme übersetzt?
  javac Hallo.java --> Bytecode Hallo class
  java Hallo (Programm wird nun ausgefuehr)
1. Was ist der Java-Bytecode und wozu dient er?  
   Java-Bytecode ist eine Plattfirm unabhaengige Code, welcher Java-Quellcode darstellt.
   Dieser Bytecode ist Portabel, da dier Code von einer einer Virtuellen Maschine kompiliert und ausgefuehrt wird.
1. Was ist die JVM und was macht sie?
   Die JVM ist ein isoliertes System auf denen die Java Programme kompiliert und ausgefuehrt werden.
   Dadurch wird der Rechner vor systemkritischen Operationen und potenziell schädlichem Code geschuetzt.  
   Nachteil ist das Zugriffe auf Hardware Komponenten erschwert ist, jedoch werden so kritische Systemressourcen  geschuetzt.
   Die JVM kann Hotspots ermitteln und in diesen Faellen den Just-In-Time Compiler nutzen um den Maschinencode zur Laufzeit zu optimieren.
## Java Programme 
1. Wie können Sie eine Java Applikation erstellen?
   Wie muessen uns eine JDK dowloaden, da wir bestimmte Entwicklungstools benoetigen sowie einen Java-Compiler.  
   Zudem brauchen wir eine JVM zudem waeren Bibliotheken nuetzlich, deswegen bracuhen woir auch ein JRE welches inclusiv mit der JDK heruntergeladeb wird.
   Nun ein Textdoukument mit endung.java erstellen und dann nur noch kompilieren und ausfuehren.
2. Wie viele main-Funktionen können Sie in ihrem Programm haben?  
   Mehrere aber, nur die Main der Klasse wird beruecksichtigt, welche zum starten des Programms genutzt wurde.  
## Klassen und Objekte  
1. Wozu dient final? <br>
   **Methoden**: Methoden koennen nicht ueberschrieben werden durch unterklassen  
   **Klassen**: Von der Klasse kann nicht geerbt werden  
   **Variablen**: Variablen werden zu Konstanten und koennen nicht mehr geaendert werden
1. Referenzen (Was sind Referenzen in Java?)<br>
   Eine Referenz ist ein Verweis der auf einen Speicherbereich eines Objektes zeigt.  
1. Gibt es Pointer in Java?<br>
   Klassiche Pointer die man aus C oder C++ gibt es nicht, jedoch haben wir Referenzen die nur im Bezug von Klassen und Objekten gibt. 
1.  Speicher freigeben?
   Speicher kann nur implizit freigeben werden in dem man zum Beispiel Out-Of-Scope geht oder keine Referenz auf ein Objekt mehr besitzt.
   Dadurch das es keine Referenz mehr auf das Objekt existiert wird der Speicherbereich des Objekts freigegeben.
   Diese Freigabe wird durch den Garbage Collector durchgefuehrt.
## Wiederverwendbarkeit
1. Welche Arten von Vererbung gibt es in Java?
  - Einfach Vererbung einer Superklasse -> Ist-Ein-Beziehung
1. Statische vs. dynamische Bindung
  Bei der dynamischen Bindung wird die Methode zur Laufzeit basierend auf dem tatsächlichen Typ des Objekts aufgelöst.
  Bei der statischen Bindung wird die Methode zur Übersetzungszeit basierend auf dem Typ der Referenz aufgelöst.
  Diese Dynamische Bundung wird auch als Polymorphie bezeichnet. In Java wird standardmaessig die Dynamische Bindung angewendet.
1. Gemeinsame Oberklasse?
   **to be continued**
1. Konzept, was ist drin in einem Paket?
   Pakete dienen dazu Quellcode und class-Dateien zu trennen, dadurch ist das Projekt uebersichtlicher.
   Pakete sind Seperate Ordner die Quellcode und oder oder uebersetzte Klassen besitzt.
1. Standard-Pakete von Java
   java.util, java.awt und javax.swing
1. Erläutern Sie die folgende Codezeile. Was bedeuten die einzelnen Komponenten und was wird (warum) passieren?<br>  
   `java.lang.System.out.println(“this = “ + this);`<br>
   Wir Importieren die Klasse System aus dem Paket java.lang. 
   Von der statischen Instanzvariable 'out' von der Klasse PrintStream rufen wir die statische Methode println() auf, welche uns einen String an die Standard-Ausgabe   ausgibt.
   'this =' wird mit dem einem String konkatiniert, welcher aus der toString Methode der aktuellen Instanz erzeugt wird.   
   
   
### Spickzettel
1. Bedeutung Interaktiver Systeme  
      • Steigende Anzahl Anwender
      • Private Nutzung gewann in den letzten Jahren immer mehr
      an Bedeutung
      • Private Nutzer können in der Regel nicht geschult werden
      • Alle Benutzergruppen müssen mit verschiedensten
      Systemen arbeiten können (barrierefreie Nutzung muss
      ermöglicht werden)
      • Webbasierte Systeme müssen auf verschiedensten Geräten
      nutzbar sein (Mobile, Tablet, Desktop)
1. Aspekte Interaktiver Systeme <br>
      Mensch– Wahrnehmen– Denken– Handeln– Eigenschaften berücksichtigen
      Maschine– Wahrnehmen / Eingeben– Verarbeiten / Reagieren– Darstellen / Ausgeben– Eigenschaften konstruierbar
1. Software-Ergonomie:
      Ziel: Arbeit hin zu leicht verständlicher und schnell benutzbarer Software<br>
      – unter den gebotenen technischen Möglichkeiten – und unter der Einhaltung definierter bzw. empirisch
      entstandener Standards und Styleguides<br>
      • Teilgebiet der Mensch-Computer-Interaktion
      • Ergebnis ist die Gebrauchstauglichkeit von Computerprogrammen
      Konsistenz der Benutzerführung-Ständige Verfügbarkeit-Unmittelbare Verständlichkeit der Benutzerführung-Automatisierung sich wiederholender Aufgaben
1. Richtlinien <br>
   Ziel:• konsistente Benutzungsschnittstellen<br>
  Inhalte:• Absprache mit Kunden / Zielgruppe • Handlungsrahmen für Entwickler(gruppen)<br>
  • Berücksichtigung allgemein gültiger Regeln, Normen, Standards und gesetzlicher Regelungen <br>
1. Normen <br>
     **Aufgabenangemessenheit:** aufgabenangemessen wenn Benutzer unterst., seine Arbtsauf. eff u. eff zu er.<br>
     **Erwartungskonformität:** erw.konform wenn konsistent ist und den Merkmalen des Benutzers entspricht<br>
     **Lernförderlichkeit:** lernfeorderlich wenn Benutzer beim Erlernen des Dialogsystems unterstützt und anleitet.<br>
     **Selbstbeschreibungsfähigkeit:** selbstbeschreibungsfähig wenn je. einz. Dia.Schr. d. Rueck. des DiaS. unm. verst. ist oder auf An.von B. er. wir.<br>
     **Fehlertoleranz:** akzeptabeles Ergebnis trotz durch korrektur von benutzerfehlern<br>
     **Steuerbarkeit:** steuerbar wenn starten richtung u. geschw. beeinflussen<br>
     **Individualisierbarkeit:** wenn DiaS Anpass an Erfo. der Arbe. sowi anp an ind. skills und Vorl. des B zul.
   <br>
Anspruch Erwartungskonformität:
– Fördert Standardisierung und Vereinheitlichung
• Ansprüche, Individualisierung und Lernförderlichkeit
– Berücksichtigung spezifischer Ausprägungen
– Lernprozesse
• Scheinbarer Widerspruch? Nein:
– UI soll Gewohnheiten unterstützen und
– Erlernen neuer Methoden, Entwickeln individueller Lösungswege
unterstützen
1. Barrierefreiheit
technische Zugänglichkeit der Software verbunden mit grundlegenden
Prinzipien der Software-Ergonomie<br>
• Ziele
 – Software durch jeden Benutzer einsetzbar
• „Keinen Nutzer von der Nutzung ausschließen“
• Nutzung durch Behinderte ohne besondere Erschwernis und fremde Hilfe
– Produktivität erhöhen
– Zufriedenheit erhöhen
1. Farbfehlsichtigkeiten
   rot-gelb, braun-gruen, violett-blau, dunkelrot-schwarz
   - Protonapie: Rot-Zapfen fehlt 
   - Protanomalie: Rotsehschw. Rot-Zapfen degeneriert
   - Deutanopie: Gruen-Blindheit dunkelrot-schwarz nicht vertasucht
   - Deutanomalie: Gruensehschwaeche
     
