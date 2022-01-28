# body mass index calculator
```java
import java.util.Scanner;
public class train {
    public static void main(String[] args){
        /*
        * body mass index
        * formula = mass(kg)/height^2(m)
        */
        Scanner scn = new Scanner(System.in);
        double weight,height,result;

        System.out.print("please enter weight(kg) : ");
        weight = scn.nextDouble();
        System.out.print("please enter height(m) : ");
        height = scn.nextDouble();

        result = weight / Math.pow(2,height);

        System.out.println("Your body mass index is "+result);
        
        if(result < 18.5){
            System.out.println("under average weight");
        }
        else if(result > 18.5 && result < 25 ){
            System.out.println("normal weight");
        }
        else if(result > 25 && result < 30){
            System.out.println("above average weight");
        }
        else{
            System.out.println("obesity");
        }


    }
}
```