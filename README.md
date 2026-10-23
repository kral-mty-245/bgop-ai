<h1 align="center">Projede Yer Alan ve Yönetenler:
Muhammed Taha Yeşilkır - https://github.com/kral-mty-245</h1>
<p align="center">
  <img src="https://media.base44.com/images/public/6a3d316877e69ab6f30854db/e0ef1f6f6_Gemini_Generated_Image_cpbfmbcpbfmbcpbf.png" alt="Beşiktaş Gazi Osman Paşa Ortaokulu logosu" width="150">
</p>

<h1 align="center">BGOP AI</h1>

<p align="center">
  Beşiktaş Gazi Osman Paşa Ortaokulu için geliştirilen yapay zekâ destekli eğitim platformu
</p>

<p align="center">
  <a href__="https://bgopai.base44.app/indir"><strong>Uygulamayı İndir ve Kurulum Bilgilerini Gör</strong></a>
</p>

---

## BGOP AI nedir?

**BGOP AI**, Beşiktaş Gazi Osman Paşa Ortaokulu öğretmen ve öğrencilerinin eğitim süreçlerini desteklemek amacıyla geliştirilen bir eğitim platformudur. Ders içerikleri ve sınıf etkinliklerinin hazırlanmasına yardımcı olan yapay zekâ destekli araçlar sunar.

Platformun web sürümüne doğrudan [bgopai.base44.app](https://bgopai.base44.app) adresinden erişilebilir. Pardus/Linux ve Windows masaüstü uygulamalarının indirme seçenekleri ile güncel kurulum yönergeleri için [Uygulamayı İndir](https://bgopai.base44.app/indir) sayfasını ziyaret edin.

> BGOP AI, öğretmen denetiminde kullanılan okul içi bir pilot eğitim aracıdır. MEB, EBA veya MEBİ ile resmî bir entegrasyonu ya da onayı olduğu anlamına gelmez.

## Öne çıkan özellikler

- **Tasarım Stüdyosu:** Ders sunumları hazırlamaya ve düzenlemeye yardımcı olur.
- **Sınav Sihirbazı:** Ders ve konuya yönelik açık uçlu soru içerikleri oluşturmayı destekler.
- **Sınıf Sohbeti:** Öğretmenlerin sınıf içi öğrenme süreçlerinde kullanabileceği yapay zekâ destekli sohbet alanı sunar.
- **Medya Stüdyosu:** Eğitim amaçlı görsel ve medya içerikleri hazırlamaya yardımcı olur.
- **Sınıf Araçları:** Sınıf etkinliklerinde kullanılabilecek araçlar sağlar.
- **Öğrenci alanı:** Öğrencilerin kendileri için sunulan etkinlik ve ödevlere erişmesini destekler.

Yapay zekâ tarafından oluşturulan içerikler kullanılmadan önce öğretmen tarafından gözden geçirilmelidir.

## Kolay kurulum

### 1. Cihazınıza uygun paketi bulun

[https://bgopai.base44.app/indir](https://bgopai.base44.app/indir) adresini açın ve kullandığınız cihaza uygun bölümü seçin:

- **Pardus / Linux:** AppImage veya `.deb` paketi
- **Windows:** Kurulum `.exe` dosyası

> İndirme sayfasında bir paket “hazırlanıyor” olarak görünüyorsa o platform için indirilebilir dosya henüz yayımlanmamıştır. Paket yayımlandığında bağlantı aynı sayfada görünecektir.

### 2. Pardus / Linux kurulumu

**`.deb` paketi:**

1. İndirme sayfasından Pardus/Linux `.deb` dosyasını indirin.
2. İndirilen dosyaya çift tıklayın.
3. Açılan paket kurucusundaki yönergeleri izleyerek kurulumu tamamlayın.
4. Uygulamayı uygulama menüsünden açın.

**AppImage paketi:**

1. İndirme sayfasından AppImage dosyasını indirin.
2. Dosyaya sağ tıklayıp **Özellikler** bölümünü açın.
3. **İzinler** sekmesinden dosyanın program olarak çalıştırılmasına izin verin.
4. Dosyaya çift tıklayarak BGOP AI’yi başlatın.

Pardus sürümüne ve masaüstü ortamına göre menü adları değişebilir. Dosya çalıştırılamıyorsa okulunuzun teknik destek sorumlusundan yardım alın.

### 3. Windows kurulumu

1. İndirme sayfasından Windows `.exe` kurulum dosyasını indirin.
2. İndirilen dosyaya çift tıklayın.
3. Windows güvenlik onayı gösterirse, dosyayı yalnızca indirme sayfasındaki resmî bağlantıdan indirdiğinizi doğruladıktan sonra kuruluma devam edin.
4. Kurulum tamamlandığında BGOP AI’yi Başlat menüsünden veya masaüstü kısayolundan açın.

## İnternet bağlantısı

Masaüstü uygulaması BGOP AI web platformunu açar. Uygulamanın çalışması ve çevrim içi özelliklerin kullanılabilmesi için internet bağlantısı gerekir.

## Geliştiriciler için: masaüstü paketlerini oluşturma

Bu depo, BGOP AI web platformunu Electron penceresinde açan masaüstü uygulamasını ve GitHub Actions ile paket oluşturma iş akışını içerir.

### Gereksinimler

- Node.js 20
- npm
- GitHub deposunda GitHub Actions’ın etkin olması

### Yerel geliştirme

Depoyu bilgisayarınıza indirin ve proje klasöründe şu komutları çalıştırın:

```bash
npm install
npm start
Kurulum dosyalarını oluşturma
Linux için AppImage ve .deb paketleri:

npm run dist:linux
Windows için kurulum .exe dosyası:

npm run dist:win
Paketler dist klasörüne oluşturulur. Linux ve Windows paketlerinin kendi işletim sistemlerinde derlenmesi önerilir.

GitHub Actions ile otomatik derleme
İş akışı deposuna eklenip GitHub Actions etkinleştirildiğinde, main dalına yapılan gönderimler otomatik derlemeyi başlatır. Derleme tamamlandığında:

Linux için AppImage ve .deb
Windows için .exe
dosyaları GitHub Actions çalıştırmasının Artifacts bölümünde bulunur. GitHub Release oluşturulmuşsa dağıtım dosyaları ilgili sürümün Releases bölümünde de yer alır.

Sürüm yayımlarken package.json ve GitHub Actions iş akışındaki sürüm etiketinin birbiriyle uyumlu olduğundan emin olun.

Güvenlik ve sorumlu kullanım
Kurulum dosyalarını yalnızca resmî indirme sayfasından veya bu depoda yayımlanan resmî GitHub Releases bölümünden indirin.
Öğrenci bilgilerini herkese açık depolara, ekran görüntülerine veya destek taleplerine eklemeyin.
Yapay zekâ çıktıları hata içerebilir. Eğitim materyallerini ve değerlendirme sorularını kullanmadan önce öğretmen kontrolünden geçirin.
BGOP AI’nin resmî MEB/EBA/MEBİ entegrasyonu veya onayı bulunmamaktadır.
İndirme ve erişim
Masaüstü uygulaması ve kurulum yönergeleri: bgopai.base44.app/indir
Web uygulaması: bgopai.base44.app
Lisans
Bu depoda ayrıca bir lisans dosyası yayımlanmadıysa, kodun yeniden kullanımı ve dağıtımı için izin verildiği varsayılmamalıdır. Lisans bilgisi gerektiğinde depo sahibine danışın.

#BGOP AI
