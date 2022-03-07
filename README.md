# Manav Kasa Programı
Patika.dev > Java101 > Ödev2 - Manav Kasa Programı

## Java ile kullanıcıların manavdan almış oldukları ürünlerin kilogram değerlerine göre toplam tutarını ekrana yazdıran programı yazın.

### Meyveler ve KG Fiyatları
- Armut : 2,14 TL
- Elma : 3,67 TL
- Domates : 1,11 TL
- Muz: 0,95 TL
- Patlıcan : 5,00 TL

		import java.util.*;
		
		public class odev2 {

			public static void main(String[] args) {
				// Yeni bir tarayıcı(scanner) oluştur.
				Scanner sc = new Scanner(System.in);
		
				// Kullanıcıdan kilo değerlerini al.
				System.out.println("Armut kaç kilo? : ");
				int armut = sc.nextInt();
		
				System.out.println("Elma kaç kilo? : ");
				int elma = sc.nextInt();
		
				System.out.println("Domates kaç kilo? : ");
				int domates = sc.nextInt();
		
				System.out.println("Muz kaç kilo? : ");
				int muz = sc.nextInt();
		
				System.out.println("Patlıcan kaç kilo? : ");
				int patlıcan = sc.nextInt();
		
				// Ürünlerin kilogram değerlerine göre tutarlarını gir.
				final double armutKg = 2.14;
				final double elmaKg = 3.67;
				final double domatesKg = 1.11;
				final double muzKg = 0.95;
				final double patlıcanKg = 5.00;
		
				// Toplam tutarı hesapla.
				double toplam = (armutKg * armut) + (elmaKg * elma) + (domatesKg * domates)
						+ (muzKg * muz) + (patlıcanKg * patlıcan);
		
				//Toplam tutarı yazdır.
				System.out.println("Toplam Tutar: " + toplam);
			}
		}
