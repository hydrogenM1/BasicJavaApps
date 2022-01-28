# basic atm project

```java
import java.util.Scanner;
public class train {
    public static void main(String[] args){
       /*ATM projesi
            1.transaction balance inquiry
            2.withdraw money
            3.deposit money
       */

        Scanner sc = new Scanner(System.in);
        // ondecen belirlenmis balance
        double balance = 1000;
        String transaction = "   1.balance inquiry\n" + 
        "   2.Withdraw Monei\n" 
        + "   3.Para Yatirma\n" + 
        "   4.Quit\n";

        System.out.println("*************************");
        System.out.print(transaction);
        System.out.println("*************************");


        while(true){
            System.out.print("Please select the transaction : ");
            String operation = sc.nextLine();

            if(operation.equals("4")){
                System.out.println("Quitting");
                break;
            }
            else if(operation.equals("1")){
                System.out.println("your balance : "+ balance);
            }
            else if(operation.equals("2")){
                System.out.print("Please enter the amount you wish to withdraw : ");
                double amount = sc.nextDouble();
                sc.nextLine();
                if(balance - amount < 0){
                    System.out.println("insufficient balance...\n your balance : "+balance);
                }
                else{
                    double newBalance = balance - amount;
                    balance = newBalance;
                    System.out.println("Cekilen amount : "+amount+"\n"+"Kalan balanceniz : "+balance);
                }
            }
            else if(operation.equals("3")){
                System.out.print("Please enter the amount you wish to deposit : ");
                double amount = sc.nextDouble();
                sc.nextLine();
                if(amount < 0 ){
                    System.out.println("Please enter valid amount.");
                }else{
                    double newBalance = amount + balance;
                    balance = newBalance;

                    System.out.println("Deposit amount : "+ amount + "\n" + "New balance : " + balance);
                }
            }
        }

    }
}
```