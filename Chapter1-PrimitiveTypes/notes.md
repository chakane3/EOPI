# Primitive Types

The most basic building block of programming languages are ```variables```. Variables can have ```types```. We'll often deal with these primitive types such as: float, long, int, string, char, obj. These types take up different amount of memory since were storing bits here. When you do ```int i = 10;```  the program will allocate some memory for your integer. Take an example of a program that counts bits. 

<details>
    <summary>countBits.java</summary>
    
```java
public class countBits {
    public static void main(String[] args) {
        System.out.println(countBits(293847532));
    }

    public static short countBits(int x) {
        short numBits = 0;
        while(x != 0) {
            numBits += (x & 1);
            x >>>= 1;
        }
        return numBits;
    }
}
```
</details>
