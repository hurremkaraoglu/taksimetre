# taksimetre



// KM başına 2.20 TL
// Minimüm ödenecek tutar : 20 TL
// Taksimetre Açılış 10 TL


import java.util.Scanner;
public class taksimetre {
    public static void main(String[] args) {
        int km;
        double perKm = 2.20, total = 10;

        Scanner input=new Scanner(System.in);
        System.out.print("Mesafeyi KM cinsinden giriniz : ");
        km = input.nextInt();

        total += (km * perKm);

        total =(total < 20) ? 20 : total;

        System.out.println("Ödenecek tutar : " + total);
    }
}
