# GIT

git komutları kullanımını ve açıklamalarını içerir

## Komutlar

1. `git config --global user.name "ad soyad"`
    - git commitlerinde görünecek yazar kimliğinin ad değerini global olarak belirler
    - yapılan değişikliklerin kimin tarafından yapıldığını göstermek içindir

2. `git config --global user.email "email"`
    - git commitlerinde görünecek yazar kimliğinin email değerini global olarak belirler
    - yapılan değişikliklerin kimin tarafından yapıldığını göstermek içindir

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
    
10. `git checkout ID/HASH`
    - id: commit'e ait benzersir anahtar
    - geçmişteki commit versionlarına dönmeyi sağlar


### BRANCHING AND MERGING (DALLANMA VE BİRLEŞTİRME)

#### BRANCHING (DALLANMA)

bir projede paralel olarak bağımsız geliştirmeye olanak tanır
örneğin:
projeye X özelliğini ayrı bağımsız bir dalda geliştirmeni sağlar

> [!NOTE]
> `test-projesi` adı ile örnek proje oluşturdum, içeriği 3 dosyadan 1 dosyaya birleştirmek için `one-file` adında bir dal oluşturdum

11. `git branch dal-adi`
    - yeni bir dal oluşturur

12. `git branch`
    - dalları listeler
    
13. `git checkout dal-adi`
    - belirtilen dal'a geçer
    
14. `git push origin dal-adi`
    - yaptığınız değişikliklerin belirtilen ve istenilen dal'a aktarır


#### MERGING (BİRLEŞTİRME)

bir projede paralel olarak bağımsız geliştirilen dallanmaları birleştirir
örneğin:
projeye X özelliğini ayrı bağımsız bir dalda geliştirilen başka bir dalla birleştirir
