## basic interest calculator
```java
import java.util.Scanner;
public class train {
    public static void main(String[] args){
/*
*   Interest Calculator
*
*   Enter main money :
*   Enter how many years do you want maturity :
*
*   note: interest percentage %6
*
*   1.year main money:----------
*   2.year main money:----------
*   3.year main money:----------
*           .
*           .
*           .
*           .
*           .
*           .
*  n.year main money:----------
*
*
*/
        Scanner scan = new Scanner(System.in);
        double interestPercentage = 0.06;
        System.out.print("Enter main money : ");
        double mainMoney = scan.nextDouble();
        System.out.print("Enter how many years do you want maturity ");
        double termTime = scan.nextDouble();
        // ,=,e
        double newMainMoney;
        newMainMoney = mainMoney;
        double interest = 0;

        for(int i = 1; i <= termTime; i++){
            interest = newMainMoney * interestPercentage;
            newMainMoney += interest;
            System.out.println("end of "+i+". year main money "+newMainMoney);
        }
    }
}
```