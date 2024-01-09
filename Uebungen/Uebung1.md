### Was ist die Ausgabe des folgenden Java Codes?
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
