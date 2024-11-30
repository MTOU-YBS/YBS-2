package ogrenciNot;
 
    class deneme {
        String isim;
        int not;
    
        public deneme(String isim, int not) {
            this.isim = isim;
            this.not = not;
        }
    }
    
    class  den1{
        deneme veri;
        den1 nextTimeBoomer;
    
        public den1(deneme veri) {
            this.veri = veri;
        }
    }   
    
    class liste {
        den1 ilk;
    
        public void ekleOgrenci(String isim, int not) {
            den1 fer = new den1(new deneme(isim, not));
            if (ilk == null) {
                ilk = fer;
            } else {
                den1 Ferhat = ilk;
                while (Ferhat.nextTimeBoomer != null) Ferhat = Ferhat.nextTimeBoomer;
                Ferhat.nextTimeBoomer = fer;
            }
        }
    
        public void toplamOgrenci() {
            if (ilk == null) {
                System.out.println("liste bos");
                return;
            }
            den1 Ferhat = ilk, toplamSeviye = ilk;
            while (Ferhat != null) {
                if (Ferhat.veri.not > toplamSeviye.veri.not) toplamSeviye = Ferhat;
                Ferhat = Ferhat.nextTimeBoomer;
            }
            System.out.println("en başarılı : " + toplamSeviye.veri.isim + ", not: " + toplamSeviye.veri.not);
        }
    }
    
    public class soru1 {
        public static void main(String[] args) {
            liste liste = new liste();
            liste.ekleOgrenci("Ferhat", 64);
            liste.ekleOgrenci("Zöhre", 49);
            liste.ekleOgrenci("Anıl", 90);
            liste.ekleOgrenci("Beyza", 90);
            liste.ekleOgrenci("Yiğit", 90);
            liste.toplamOgrenci();
        }
    }

