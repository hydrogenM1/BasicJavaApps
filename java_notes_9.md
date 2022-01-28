## Basic calculator with methods

```java
/*basic calculator with methods(functions)*/

import java.util.Scanner;
public class train {
    public static void addition(){
        // addition method
        System.out.print("Please enter two integer : ");
        Scanner scan = new Scanner(System.in);
        int a = scan.nextInt();
        int b = scan.nextInt();
        int sum;
        sum = a + b;
        System.out.println("result = "+ sum);
    }
    public static void multiply(){
        // multiply method
        System.out.print("Please enter two integer : ");
        Scanner scan = new Scanner(System.in);
        int a = scan.nextInt();
        int b = scan.nextInt();
        int sum;
        sum = a * b;
        System.out.println("result = "+ sum);
    }
    public static void subtraction(){
        // subtraction method
        System.out.print("Please enter two integer : ");
        Scanner scan = new Scanner(System.in);
        int a = scan.nextInt();
        int b = scan.nextInt();
        int sum;
        sum = a - b;
        System.out.println("result = "+ sum);
    }
    public static void division(){
        // division method
        System.out.print("Please enter two integer : ");
        Scanner scan = new Scanner(System.in);
        int a = scan.nextInt();
        int b = scan.nextInt();
        int sum;
        sum = a / b;
        System.out.println("result = "+ sum);
    }
    public static void main(String[] args){
        System.out.println("MENU\nAddition[+]\nSubtraction[-]\nMultiply[*]\nDivison[/]\n");
        System.out.print("Please choose the process you want to do : ");
        Scanner scn = new Scanner(System.in);
        String process = scn.nextLine();

        switch(process){
            case "+":
                addition();
                break;
            case "-":
                subtraction();
                break;
            case "*":
                multiply();
                break;
            case "/":
                division();
                break;
        }

    }
}
```