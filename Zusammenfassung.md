
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
   ur die Main der Klasse wird beruecksichtigt, welche zum starten des Programms genutzt wurde.
