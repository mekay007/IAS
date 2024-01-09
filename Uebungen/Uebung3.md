# Exceptions 
### Vertstaendnis
#### 1. Analysieren Sie den Ablauf des vorstehenden Programms. Was wird jeweils ausgegeben? 
```java
import java.awt.AWTException;
public class ExceptionTest {
  public static void main(String[] args) {
     System.out.println("Anfang main");
     ExceptionTest ex = new ExceptionTest();
     ex.run();
     System.out.println("Ende main");
   }
  
  void run() {
     System.out.println("Anfang run");
     try {
       System.out.println("Anfang try-Block");
       int index = -1; // Test: -1 / 0 / 1 / 2
       final String[] args = { "OK", "NULL", null };
       String value = args[index];
       doRiskyStuff(value);
       System.out.println("Ende try-Block");
     }
     catch (IndexOutOfBoundsException ex) {
       System.out.println(
      "catch IndexOutOfBoundsException");
     }
     catch (AWTException ex) {
       System.out.println("catch AWTException");
     }
     finally {
       System.out.println("finally");
     }
     System.out.println("Ende run");
   }
  
  void doRiskyStuff(String value) throws AWTException
  {
    System.out.println("Anfang doRiskyStuff");
    if (value.toLowerCase().equals("null")) {
      System.out.println("werfe Exception");
      throw new AWTException("simuliere AWT Fehler");
    }
    System.out.println("Ende doRiskyStuff");
   }
} 
```
a) Ausgabe für **index = ‐1** <br>
b) Ausgabe für **index = 0** <br>
c) Ausgabe für **index = 1** <br>
d) Ausgabe für **index = 2** <br>

### 2. Schreiben Sie eine eigene Klasse MeineException. Welche Klasse muesen Sie erweitern?
### 3. Werfen und fangen Sie MeineException.
### 4. Wie koennen Sie die generische Exception benutzen um MeineException zu fangen.
### 5. Wie koennen Sie sich die Exceptioninfo ausgeben lassen.(Hinweis: Polymorphie)
