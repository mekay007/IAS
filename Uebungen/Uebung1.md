### 1. Nennen Sie alle Schritte von einem Javaprogramm von Erstellung bis zur Aufuehrung. Und erlauteren Sie diese kurz.
### 2. Was ist eine JVM und was sind ihre Vorteile un Nachteile?
### 3. Was ist der  unterschied zwischen JRE und JDK und was davon ist noetig fuer den Entwickler bzw. Anwender?
### 4. Muss jede Klasse in einer eigenen Datei sein?
### 5. Welche der folgenden Java‐Anweisungen sind fehlerhaft? Handelt es sich um einen Compiler‐ oder einen Laufzeitfehler? 
```java
class C {
 public static void main(String[] args) {
   short s = 7;
   int i = -12;
   unsigned int u = +12;
   long l = 123456789;
   float f = 3.1415;
   double d = 3.1415;
  
   s = i;
   i = s;
   s = 123456789;
   int i2 = (int) l;
   i = 12.4;
   i = 12L;
   i = (int) 12L;
   String str = "Hallo" + "Welt";
   str = args[-3];
   str = "i = " + i;
   str = str - i;
  
   boolean b = false;
   b = 12L == 12;
 }
}
```
### 6. Was ist die Ausgabe des folgenden Java Codes?
  ```java
  class A{
    private int val;
    public A(int n){
        val=n;
    }
    public void setVal(int val) {
        this.val = val;
    }
    public int getVal() {
        return val;
    }

    public String toString() {
        return ""+val;
    }
    public boolean equals(Object obj) {
        if (this.val!=((A)obj).val)
            return false;
        return true;
    }
}

public class C {
    public static void main(String[] args) {
        A a1=new A(3);
        A a2= a1;

        a1.setVal(a1.getVal()+3);
        a2.setVal(a2.getVal()-4);

        System.out.println("A1 ="+a1.getVal());
        System.out.println("A2 ="+a1.getVal());
        System.out.println(a1.equals(new C()));

    }
}
  ```
### 7. Schreiben Sie ein einfaches Zahlen Raten das von 1-10. Falls die angegeben Zahl ausserhalb des definierten Bereiches liegt geben Sie einen Fehler mittel der Standard Fehlerausgabe aus.

