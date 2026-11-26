#  GitHub Profil Analizörü

## Problem ve Hedef Kullanıcı
İşe alım yapan kişiler, takım liderleri ve staj/iş arayan öğrenciler bir yazılımcının GitHub profilini incelerken repoları tek tek açmak zorunda kalıyor. Kişinin hangi dilleri kullandığı ve hangi projelerinin öne çıktığı hızlıca görülemiyor. Bu uygulamaya bir **GitHub kullanıcı adı** yazmak yeterli. Uygulama **GitHub API** üzerinden profil bilgilerini, en popüler repoları ve dil dağılımını tek ekranda özetliyor.

## Proje Panosu
 [GitHub Projects Panosu](https://github.com/users/eylemars/projects/2)

## Kullanılan Teknolojiler
- HTML, CSS, JavaScript (kütüphane yok)
- [GitHub REST API](https://docs.github.com/en/rest) (API anahtarı gerektirmez)

## Çalıştırma Adımları
**Seçenek 1: Canlı demo**
 https://eylemars.github.io/github-analiz/

**Seçenek 2: Yerelde çalıştırma**
1. Depoyu indirin: `git clone https://github.com/eylemars/github-analiz.git`
2. `index.html` dosyasını tarayıcıda açın.
3. Kurulum gerekmez. İnternet bağlantısı yeterlidir.

> Not: GitHub API, anahtarsız kullanımda saatte 60 istek sınırı uygular. Sınır dolarsa uygulama bunu ekranda bildirir.

## Özellikleri Deneme

### Özellik 1: Profil Kartı
- Arama kutusuna `torvalds` yazıp **Analiz Et** butonuna basın. Profil fotoğrafı, isim, biyografi, repo ve takipçi sayıları ile katılım yılı görünür.
- `bu-kullanici-yok-12345xyz` yazın. **"Kullanıcı bulunamadı."** uyarısı çıkar.
- Kutuyu boş bırakıp butona basın. **"Lütfen bir kullanıcı adı yazın."** uyarısı çıkar.

### Özellik 2: Repo ve Dil Analizi
- `torvalds` ya da `musanmaz` aratın. Profil kartının altında şunlar görünür:
  - **En Popüler 5 Repo:** yıldız sayısına göre büyükten küçüğe sıralanır. Her repoda açıklama, yıldız ve  fork sayısı yer alır.
  - **Dil Dağılımı:** repolarda kullanılan diller yüzde olarak çubuk grafikle gösterilir.
