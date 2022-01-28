## Klavyeden girilen bir sayinin Armstrong sayisi olup olmadini kontrol eden program

```java
import java.util.Scanner;
public class train {
    public static void main(String[] args){
       /* klavyeden girilen bir sayinin armstrong sayisi olup olmadigini kontrol eden program*/
        System.out.print("Bir sayi giriniz : ");
        Scanner scn = new Scanner(System.in);
        int sayi = scn.nextInt();
        System.out.print("Basamak degerini giriniz : ");
        int basamakSayisi = scn.nextInt();

        int gecici_sayi = sayi;
        int toplam = 0;

        do{
          int basamakDegeri = gecici_sayi % 10;
          gecici_sayi /= 10;

          toplam += Math.pow(basamakDegeri,basamakSayisi);
        }while(gecici_sayi > 0);

        if (toplam == sayi){
            System.out.println("Girilen sayi bir Armstrong sayisidir...");
        }
        else{
            System.out.println("Girilen sayi bir Armstrong sayisi degildir");
        }
    }
}

```