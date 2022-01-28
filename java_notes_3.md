# grade calculator

```java
import java.util.Scanner;
public class train {
    public static void main(String[] args){

        Scanner scanner = new Scanner(System.in);
        double midterm1,midterm2,totalGrade;
        double finals;

        System.out.print("lutfen vize1 , vize2 ve final sonuclariniz giriniz : ");
        midterm1 = scanner.nextDouble();
        midterm2 = scanner.nextDouble();
        finals = scanner.nextDouble();

        totalGrade = (midterm1 * 20 / 100) + (midterm2 * 30 / 100) + (finals * 50 / 100);

        if (totalGrade >= 90){
            System.out.println("Harf notunuz AA");
        }
        else if (totalGrade >= 85 && totalGrade < 90){
            System.out.println("Harf notunuz BA");
        }
        else if (totalGrade >= 80 && totalGrade < 85){
            System.out.println("Harf notunuz BB");
        }
        else if (totalGrade >= 75 && totalGrade < 80){
            System.out.println("Harf notunuz CB");
        }
        else if (totalGrade >= 70 && totalGrade < 75){
            System.out.println("Harf notunuz CC");
        }
        else if (totalGrade >= 65 && totalGrade < 70){
            System.out.println("Harf notunuz DC");
        }
        else if (totalGrade >= 60 && totalGrade < 65){
            System.out.println("Harf notunuz DD");
        }
        else if (totalGrade >= 55 && totalGrade < 60){
            System.out.println("Harf notunuz DF");
        }
        else{
            System.out.println("Harf notunuz FF");
        }

    }
}


```