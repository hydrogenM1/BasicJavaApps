## system login login app

```java
import java.util.Scanner;
public class train {
    public static void main(String[] args){
    /* system login app*/
        Scanner scn = new Scanner(System.in);
        String system_username = "Ahad Can";
        String system_password = "1220";
        int rights_of_login = 3;

        while(true){
            if(rights_of_login <= 0){
            System.out.println("Your right to enter has expired...");
            break;
            }
            System.out.print("Please enter your username : ");
            String username = scn.nextLine();
            System.out.print("Please enter your password : ");
            String password = scn.nextLine();
            if (username.equals(system_username) && password.equals(system_password)){
                System.out.println("Hos geldiniz...");
            }
            else if(!password.equals(system_password) || !username.equals(system_username))
            {
                System.out.println("username or password is wrong. Please try again...");
                rights_of_login -= 1;
                System.out.println("Remaining logins : "+ rights_of_login);
            }
        }

    }
}

```
