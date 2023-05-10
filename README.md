# Kullanıcı Girişi Ödevi
- Kullanıcı adı 'patika' ve şifresi 'java123' olan bir kullanıcı girişi ekranı yapıldı. 
- Ekranda hatalı şifre sonrası kullanıcıya şifresini değiştirmek isteyip istemediğini soran bir sayfa açılır.
- Kullanıcı şifre değiştirmek istemezse giriş sonlandırılır.
- Seçimi farklı girerse hata mesajı verilir.
- Şifresini değiştirmek ister ise yeni şifresi ekrana kullanıcı tarafından girilir.
- Eğer ki yeni şifresi eski şifresi ile aynı ise ekrana hata mesajı verilir. 

```
import java.util.Scanner;

public class userName {
    public static void main(String[] args) {
        String userName , password , sifirlama ,newPassword ;
        Scanner inp = new Scanner(System.in);

        System.out.print("Kullanıcı Adınızı Giriniz : ");
        userName = inp.nextLine();
        System.out.print("Şifrenizi Giriniz : ");
        password = inp.nextLine();

        if (userName.equals("patika")&&password.equals("java123")){
            System.out.print("Başarılı Giriş Yaptınız...");
        }
        else{
            System.out.println("Hatalı Giriş Yaptınız.\nŞifrenizi Sıfırlamak İçin Ekrana \"yes\" Yazınız." +
                    "\nSıfırlamak İstemiyorsanız Ekrana \"no\" Yazınız ");
            sifirlama = inp.nextLine();

            if (sifirlama.equals("no")){
                System.out.print("Giriş Sonlandırıldı");
            }
            else if (sifirlama.equals("yes")) {
                System.out.print("Yeni Şifrenizi Giriniz : ");
                newPassword = inp.nextLine();

                if (newPassword.equals("java123")){
                    System.out.print("Hatalı Şifre Seçimi");
                }
                else {
                    System.out.print("Şifreniz Başarıyla Değiştirdiniz.");
                }
            }
            else{
                System.out.println("Hatalı Seçim Yaptınız!!!");
            }


        }

    }
}

```
---
# Patika Linkim :
<a href="https://academy.patika.dev/profile">Patika Profil Sayfam</a>
