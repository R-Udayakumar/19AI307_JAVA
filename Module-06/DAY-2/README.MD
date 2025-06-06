# Ex.No:6(B) MULTI-LEVEL INHERITANCE

## AIM:
To Develop a Java program to perform Multilevel Inheritance to calculate the area of circle..

## ALGORITHM :
1.	Start the Program.
2.	Define class `Shapes`:
-	a) Method `print_shape()` to print "Shapes Class"
3.	Define class `Circle` that extends `Shapes`:
-	a) Declare integer `rad`
-	b) Method `get()` to read `rad` from user input
4.	Define class `Area` that extends `Circle`:
-	a) Method `cal()` to calculate `result = 3.14 * rad * rad` and print "Area of Circle is " followed by `result`
5.	In `Main` class `main` method:
-	a) Create `Area` object `obj`
-	b) Call `print_shape()`, `get()`, and `cal()` on `obj` to display shape type, read radius, and calculate area
6.	End


## PROGRAM:
 ```
/*
Program to implement a MultiLevel Inheritance using Java
Developed by: Udayakumar R
RegisterNumber: 212222230163
*/
```

## Sourcecode.java:
```java
import java.util.Scanner;
class Shapes {
    public void print_Shape() {
        System.out.println("Shapes Class");
    }
}
class Circle extends Shapes {
    protected double radius;

    // Method to get radius from the user
    public void get() {
        Scanner scanner = new Scanner(System.in);
        radius = scanner.nextDouble();
    }
}

class Area extends Circle {
    public void calc() {
        double area = 3.14 * radius * radius;
        System.out.println("Area of Circle is " + area);
    }
}

public class Main {
    public static void main(String[] args) {
        Area areaObj = new Area();

        areaObj.get();          // Input radius
        areaObj.print_Shape();  // Display Shapes Class
        areaObj.calc();         // Calculate and display area
    }
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/5068a0f2-8e7a-4376-8be8-791f56836439)

## RESULT:
Thus the java program for multi-level inheritance was executed successfully.




