# afad-bookmarks
 Pardus Yüklü PC lerde Kurumsal Yapı için Mozilla ve Chrome Browserların Sık kullanılanlar güncelleyebileceğimiz Paket kodu

 ## İçindekiler:
    * Mozilla için gerekli dosya
    * Chrome için grekli dosya


## Mozilla Firefox için:
    * /home/user/.mozilla/firefox altına dosyamızı atıyoruz.
    * Dosyamızı bir firefox üzerinde sık kullanılanları hazırladığımızda oluşuyor.
    * places.sqlite dosyası

## Chrome İçin:
    * /home/user/.config/google-chrome/Default altına dosyamızı atıyoruz.
    * Dosyamızı bir Chrome üzerinde sık kullanılanları hazırladığımızda oluşuyor.
    * Bookmarks dosyası

## Komutlar:
### Yeni kullanıcılar için:
    * /etc/skel/ altına atmamız yeterli
### Var olan Kullanıcılar için:
    * find /home -type d -name ".mozilla" -exec cp /etc/skel/.mozilla/firefox/AFADv13.default/places.sqlite "{}"/firefox/AFADv13.default/places.sqlite \;
    * find /home -type d -name "google-chrome" -exec cp /etc/skel/.config/google-chrome/Default/Bookmarks "{}"/Default/Bookmarks \;

