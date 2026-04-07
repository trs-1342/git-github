# GIT

git komutları kullanımını ve açıklamalarını içerir

## Komutlar

1. `git config --global user.name "ad soyad"`
    - git commitlerinde görünecek yazar kimliğinin ad değerini global olarak belirler

2. `git config --global user.email "email"`
    - git commitlerinde görünecek yazar kimliğinin email değerini global olarak belirler

3. `git init`
    - git ayar dosyalarını indirir

4. `git status`
    - projenin durumunu/değişikliklerini gösterir/denetler
    - değişiklikler denetimden geçtiğinde boş görünür

5. `git add .`
    - proje içinde tüm değişikliklerini denetlemeden geçirir

6. `git add text.txt`
    - proje içinde belirlenen dosyanın/dosyaların değişikliklerini denetlemeden geçirir

7. `git commit -m "mesaj"`
    - `commit`: kaydet
    - `-m`: mesaj
    - denetimden geçenlerin tümünü kaydeder ve mesaj ekler.
    
8. `git commit -a -m "mesaj"`
    - `commit`: kaydet
    - `-a`: ekle
    - `-m`: mesaj
    - denetimden geçenlerin sadece daha önce eklenmiş olanları kaydeder ve mesaj ekler, yani yeni dosyaları eklemez.
    
9. `git log`
    - tutulan commit kayıtları gösterir
    
10. `git checkout ID`
    - id: commit'e ait benzersir anahtar
    - geçmişteki commit versionlarına dönmeyi sağlar
