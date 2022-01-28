## carpim tablosu (ic ice for dongusu ile)

```java

import java.util.Scanner;
public class train {
    public static void main(String[] args){
        /* Carpim tablosu */
        for (int i = 1; i < 11; i++)
        {
            System.out.println("--------- "+i+"'ler"+ " ---------");
            for (int j = 1; j <= 10 ; j++ )
            {
                int carpim = i * j ;
                System.out.println("        "+i+" * "+j+" = "+carpim);
            }
        }
    }
}

```