import java.util.Scanner;
public class sinifGecmeOdev {
    public static void main(String[] args){
        int fiz, mat, tur, kim, muzik;
        int notTopla;
        int sonuc;
        int dersToplam = 5;
        Scanner input = new Scanner(System.in);
        System.out.println("Fizik Notunuzu Giriniz");
        fiz = input.nextInt();
        System.out.println("Matematik Notunuzu Giriniz");
        mat = input.nextInt();
        System.out.println("Türkçe Notunuzu Giriniz");
        tur = input.nextInt();
        System.out.println("Kimya Notunuzu Giriniz");
        kim = input.nextInt();
        System.out.println("Müzik Notunuzu Giriniz");
        muzik = input.nextInt();
        if (fiz <0 || fiz >100){
            dersToplam--;
            fiz = 0;
        } else if (mat <0 || mat >100) {
            dersToplam --;
            mat = 0;
        } else if (tur <0 || tur >100) {
            dersToplam--;
            tur = 0;
        } else if (kim <0 || kim >100) {
            dersToplam--;
            tur = 0;
        } else if (muzik <0 || muzik >100) {
            dersToplam--;
            muzik = 0;
        }
        notTopla = fiz + mat + kim + tur + muzik;
        sonuc = notTopla / dersToplam;
        if (sonuc>=55){
            System.out.println("Sınıfı Geçtiniz");
        } else {
            System.out.println("Sınıfta Kaldınız");
        }
    }
}
