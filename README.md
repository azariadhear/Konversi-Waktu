# Konversi-Waktu
package KonversiWaktu;
import java.util.Scanner;
public class KonversiWaktu {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("KONVERSI WAKTU");
        int masukan, menit, jam, hari, bulan;
        double sisa1, sisa2, sisa3;
        System.out.print("Masukkan waktu dalam menit : ");
        masukan = input.nextInt();
        bulan = masukan/43800;
        sisa1 = masukan%43800;
        hari = (int) sisa1/1440;
        sisa2 = sisa1%1440;
        jam = (int) sisa2/60;
        sisa3 = sisa2%60;
        menit = (int) sisa3;
        System.out.println(masukan + " menit sama dengan : \n" + bulan + " bulan\n" + hari + " hari\n" + jam + " jam\n" + menit + " menit\n");
    }
}
