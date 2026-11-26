# GitHub Profil Analizörü

## Proje Hakkında
Bir yazılımcının GitHub profiline bakarken hangi dilleri kullandığını ve hangi projelerinin öne çıktığını görmek için repoları tek tek açmak gerekiyor. Bu proje, kullanıcı adı girilince GitHub API'den bilgileri çekip profil, popüler repolar ve dil dağılımını tek sayfada gösteriyor. Staj/iş arayan öğrenciler, işe alım yapanlar veya başka geliştiricilerin profillerini hızlıca incelemek isteyenler için yaptım.

## Pano
https://github.com/users/eylemars/projects/2

## Kullanılanlar
- HTML, CSS, JavaScript
- GitHub REST API (anahtar gerektirmiyor)

## Nasıl Çalıştırılır
Canlı hali: https://eylemars.github.io/github-analiz/

Bilgisayarda çalıştırmak için:
1. `git clone https://github.com/eylemars/github-analiz.git`
2. Klasördeki `index.html` dosyasını tarayıcıda açmak yeterli, kurulum yok.

Not: GitHub API anahtarsız kullanımda saatte 60 istek sınırı koyuyor. Sınır dolarsa sayfada uyarı çıkıyor.

## Özellikleri Deneme

### 1. Profil Kartı
- `torvalds` yazıp Analiz Et'e basınca profil fotoğrafı, isim, biyografi, repo/takipçi sayıları ve katılım yılı görünüyor.
- Olmayan bir kullanıcı adı (ör. `bu-kullanici-yok-12345xyz`) yazınca "Kullanıcı bulunamadı." uyarısı çıkıyor.
- Kutu boşken butona basınca "Lütfen bir kullanıcı adı yazın." uyarısı çıkıyor.

### 2. Repo ve Dil Analizi
- `torvalds` veya `musanmaz` aratınca profilin altında:
  - Yıldız sayısına göre sıralanmış en popüler 5 repo (açıklama, yıldız ve fork sayısıyla)
  - Repolarda kullanılan dillerin yüzdelik dağılımı (çubuk grafik)
