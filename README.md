import java.util.Scanner;
public class Main {
        public static void main(String[] args){
                Scanner input = new Scanner(System.in) ;

                System.out.print("Ürünün KDVsiz fiyatını giriniz :") ;
                double kdvsizFiyat, kdvliFiyat;
                kdvsizFiyat = input.nextDouble() ;
                double kdvOrani = kdvsizFiyat < 1000  ? kdvOrani = 0.18 : 0.08 ;
                System.out.println("Kdv Oranı :" + kdvOrani);

                kdvliFiyat = kdvsizFiyat + kdvOrani;
                System.out.print("kdvliFiyat :" + kdvliFiyat);
        }
}
