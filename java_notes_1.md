
```java
{
import java.util.Scanner;
public class train {
    public static void main(String[] args){
        /* girilen 3 sayidan en buyugunu bulma */

        int maxNum ;
        int firstNum,secondNum,thirdNum;
        Scanner scn = new Scanner(System.in);

        System.out.print("Please enter a three integer : ");
        // taking inputs here
        firstNum = scn.nextInt();
        secondNum = scn.nextInt();
        thirdNum = scn.nextInt();

        maxNum = firstNum;
        // finding max input
        if (maxNum < secondNum){
            maxNum = secondNum;
        }
        if (maxNum < thirdNum){
            maxNum = thirdNum;
        }
        
        System.out.println("Max number = "+ maxNum);
    }
}
}
```