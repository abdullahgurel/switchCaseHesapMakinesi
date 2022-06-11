# switchCaseHesapMakinesi
 Switch Case İle Yapılan Basit Hesap Makinesi Örneği

# if else ile yaptığım

```
import  java.util.Scanner;
public class ifElseHesapMakinesi {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        double deger1, deger2;
        int toplama = 1, cikarma = 2, carpma = 3, bolme = 4, sonuc;
        System.out.println("Hesap Makinesi Programına Hoşgeldiniz");
        System.out.print("1. Sayi Giriniz:");
        deger1 = input.nextDouble();
        System.out.print("2. Sayi Giriniz:");
        deger2 = input.nextDouble();
        System.out.print("Girilen 2 degerin islemi saglanmasi adina asagidaki islemlerden birisini girmenizi istiyoruz" +
                "(Hangi islem ise o isleme karsilik gelen sayiyi girin lutfen):" +
                "\n Toplama:1 \n Cikarma:2 \n Carpma:3 \n Bolme:4 \n Bilgi Gir : ");
        sonuc = input.nextInt();

        if (sonuc == toplama) {
            System.out.println(("Sonuc : ") + (deger1 + deger2));
        } else if (sonuc == cikarma) {
            System.out.println(("Sonuc : ") + (deger1 - deger2));
        } else if (sonuc == carpma) {
            System.out.println(("Sonuc : ") + (deger1 * deger2));
        } else if (sonuc == bolme) {
            if (deger2 !=0) {
                System.out.println(("Sonuc : ") + (deger1 / deger2));
            }else {
                System.out.println("Bir sayi sifira bolunemez");

            }
        }else {
            System.out.println("Degerlerin disinda bir sonuc girdiniz programi bastan baslatin" +
                    "ve tekrar istenen degerlerden birini giriniz.");
        }
    }
}
```

# switch case  ile yaptığım
```
import  java.util.Scanner;
public class switchCaseHesapMakinesi {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        double deger1, deger2;
        int toplama = 1, cikarma = 2, carpma = 3, bolme = 4, sonuc;
        System.out.println("Hesap Makinesi Programına Hoşgeldiniz");
        System.out.print("1. Sayi Giriniz:");
        deger1 = input.nextDouble();
        System.out.print("2. Sayi Giriniz:");
        deger2 = input.nextDouble();
        System.out.print("Girilen 2 degerin islemi saglanmasi adina asagidaki islemlerden birisini girmenizi istiyoruz" +
                "(Hangi islem ise o isleme karsilik gelen sayiyi girin lutfen):" +
                "\n Toplama:1 \n Cikarma:2 \n Carpma:3 \n Bolme:4 \n Bilgi Gir : ");
        sonuc = input.nextInt();
        switch (sonuc) {
            case 1 :
                System.out.println(("Sonuc : ") + (deger1 + deger2));
                break;
            case 2 :
                System.out.println(("Sonuc : ") + (deger1 - deger2));
                break;
            case 3 :
                System.out.println(("Sonuc : ") + (deger1 * deger2));
                break;
            case 4 :

                        boolean kosul1;
                        String result;
                        kosul1 = deger2 > 0 ;
                        result = kosul1 ? (("Sonuc: ")+(deger1/deger2)) : "Deger 0 olamaz" ;
                        System.out.println(result);
                        break;

            default:
                System.out.println("Degerlerin disinda bir sonuc girdiniz programi bastan baslatin" +
                        "ve tekrar istenen degerlerden birini giriniz.");
                break;
        }
     }
}
```
