import java.util.Scanner;
public class NotOrtalamasi {

    /* Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve
      ortalamalarını hesaplayıp ekrana bastırılan programı yazın.
      Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana
      "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.
      Not: İf Else yapısı kullanılmayacak.*/
      
    public static void main(String[] args) {
        int mat, fizik, kimya, turkce, tarih, muzik;

        Scanner inp= new Scanner(System.in);

        System.out.print("Matematik Notunuz:");
        mat = inp.nextInt();

        System.out.print("Fizik Notunuz:");
        fizik = inp.nextInt();

        System.out.print("Kimya Notunuz:");
        kimya = inp.nextInt();

        System.out.print("Turkce Notunuz:");
        turkce = inp.nextInt();

        System.out.print("Tarih Notunuz:");
        tarih = inp.nextInt();

        System.out.print("Muzik Notunuz:");
        muzik = inp.nextInt();

        int toplam = (mat + fizik + kimya + turkce + tarih + muzik);

        double sonuc = toplam/6;

        System.out.println("Ortalamaniz:" + sonuc);

        //Sınıfı geçti-Sınıta kaldı

        System.out.println(sonuc  > 60 ?"Sinifi gecti":"Sinifta kaldi");
    }}
