# JeSuis

JeSuis; avukatlık ve arabuluculuk süreçlerinde müvekkil, dosya, masraf, muhasebe, makbuz, ücret ve belge yönetimini tek masaüstü uygulamasında toplamak için hazırlanmış profesyonel bir iş takip yazılımıdır.

**Güncel sürüm:** [v0.1.0](https://github.com/hknrslnby-eng/je-suis/releases/tag/v0.1.0)

## Bu repo ne içerir?

Bu GitHub deposu yalnızca **son kullanıcı kurulum dosyalarını** ve dağıtım dokümantasyonunu içerir. Uygulamanın kaynak kodu, geliştirme ortamı ve özel yapılandırmalar burada yayımlanmaz.

Release sayfasının altında görünen **Source code (zip)** ve **Source code (tar.gz)** bağlantıları GitHub tarafından otomatik oluşturulur; bu arşivler yalnızca bu dağıtım reposunun anlık görüntüsünü (README ve lisans metni) içerir, JeSuis uygulama kaynak kodunu içermez. GitHub şu an bu otomatik arşivleri kaldırmaya izin vermez; yüklediğiniz kurulum dosyalarına etkisi yoktur.

## JeSuis ne yapar?

JeSuis, ofis içi operasyonları modüler bir yapıda bir araya getirir:

| Modül | Özet |
| --- | --- |
| **Dashboard** | Günlük özet, hızlı erişim ve genel durum görünümü. |
| **Müvekkiller** | Müvekkil kayıtları, iletişim bilgileri ve ilişkili dosya/iş bağlantıları. |
| **Taraflar** | Avukatlık ve arabuluculuk süreçlerinde karşı taraf ve ilgili kişi kayıtları. |
| **Ofis Personeli** | Personel ekleme, listeleme ve ofis içi görev dağılımı. |
| **Raporlama** | Avukat ve arabulucu akışlarında dosya/iş takibi, planlayıcı ve arabuluculuk tutanağı oluşturma. |
| **Masraf Takibi** | Dosya ve iş bazlı masraflar, tahsilatlar, ilişkili dosya havuzları. |
| **Muhasebe** | Makbuz ve gider kayıtları, muhasebe verileri; belge yüklemelerinde yerel yapay zekâ destekli alan önerisi. |
| **Ücret Takibi** | Aylık, saatlik, karma, iş bazlı, tevkil, M.İ.V.Ü, adli yardım, CMK ve arabuluculuk ücret hesapları. |
| **Belge Arşivi** | Dosya ve işlere bağlı belgelerin arşivlenmesi, aranması ve önizlenmesi. |
| **Ayarlar** | Tema, çalışma alanı, yedekleme, eşitleme ve uygulama tercihleri. |

### Veri ve gizlilik

Verileriniz öncelikle **kendi bilgisayarınızda** tutulur. JeSuis, kurulum paketine kullanıcı verisi eklemez; her kurulum kendi yerel veritabanını oluşturur. Yedekleme ve mevzuata uygun veri saklama sorumluluğu kullanıcıya aittir. Ayrıntılı bilgi için uygulama içindeki **Yasal Bilgilendirme** bölümüne bakın.

### Desteklenen platformlar

Windows, Linux ve macOS için ayrı kurulum paketleri sunulur. Yapay zekâ özellikleri kurulumla birlikte gelen yerel motora dayanır; harici model kurulumu gerekmez.

## Hangi dosyayı indirmeliyim?

| İşletim sistemi | İndirilecek dosya | Not |
| --- | --- | --- |
| Windows 64-bit | `JeSuis_0.1.0_windows_x64_setup.exe` | Önerilen kurulum dosyasıdır. |
| Windows 64-bit | `jesuis_0.1.0_windows_x64.exe` | Kurulumsuz taşınabilir sürüm. |
| Linux 64-bit | `JeSuis_0.1.0_amd64.AppImage` | Kurulum gerektirmeden çalıştırmak için. |
| Linux 64-bit | `JeSuis_0.1.0_amd64.deb` | Debian, Ubuntu ve uyumlu dağıtımlar için. |
| macOS (Intel + Apple Silicon) | `JeSuis_0.1.0_universal.dmg` | Önerilen macOS kurulum dosyasıdır. |
| macOS (Intel + Apple Silicon) | `JeSuis_0.1.0.app.zip` | DMG yerine zip tercih edenler için. |

## Terminalden indirme (v0.1.0)

Tüm dosyalar aynı release altında yayımlanır:

`https://github.com/hknrslnby-eng/je-suis/releases/tag/v0.1.0`

### Windows (PowerShell)

Kurulum dosyası (önerilen):

```powershell
Invoke-WebRequest -Uri "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/JeSuis_0.1.0_windows_x64_setup.exe" -OutFile "JeSuis_0.1.0_windows_x64_setup.exe"
```

Taşınabilir exe:

```powershell
Invoke-WebRequest -Uri "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/jesuis_0.1.0_windows_x64.exe" -OutFile "jesuis_0.1.0_windows_x64.exe"
```

### Linux (AppImage)

```bash
curl -fL -o JeSuis_0.1.0_amd64.AppImage "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/JeSuis_0.1.0_amd64.AppImage"
chmod +x JeSuis_0.1.0_amd64.AppImage
./JeSuis_0.1.0_amd64.AppImage
```

### Linux (deb)

```bash
curl -fL -o JeSuis_0.1.0_amd64.deb "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/JeSuis_0.1.0_amd64.deb"
sudo apt install ./JeSuis_0.1.0_amd64.deb
```

### macOS (DMG, önerilen)

```bash
curl -fL -o JeSuis_0.1.0_universal.dmg "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/JeSuis_0.1.0_universal.dmg"
open JeSuis_0.1.0_universal.dmg
```

### macOS (app zip)

```bash
curl -fL -o JeSuis_0.1.0.app.zip "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/JeSuis_0.1.0.app.zip"
unzip JeSuis_0.1.0.app.zip
open JeSuis.app
```

## Kurulum

### Windows

1. `JeSuis_0.1.0_windows_x64_setup.exe` dosyasını indirin.
2. Dosyayı çalıştırın.
3. Kurulum tamamlandığında JeSuis masaüstünden veya başlat menüsünden açılabilir.

### Linux

AppImage veya deb komutları yukarıdaki terminal bölümünde verilmiştir.

### macOS

1. `JeSuis_0.1.0_universal.dmg` dosyasını indirin.
2. DMG dosyasını açın.
3. JeSuis uygulamasını Applications klasörüne taşıyın.

## Kolay kurulum

JeSuis paketleri kolay indirme ve kurulum için hazırlanır. Windows kurulum dosyasını indirip çalıştırabilirsiniz. Linux için AppImage veya deb paketi, macOS için DMG paketi kullanılır.

Windows veya macOS, imzasız uygulamalarda ek bir güvenlik uyarısı gösterebilir. Bu durumda dosyayı yalnızca bu resmi GitHub adresinden indirdiğinizden emin olun:

https://github.com/hknrslnby-eng/je-suis/releases

## Güvenlik Notu

Release ile birlikte `SHA256SUMS.txt` yayımlanır. Windows ve macOS için ücretli resmi imza kullanılmaz; bu yüzden işletim sistemi ilk açılışta onay isteyebilir.

Linux örneği:

```bash
curl -fL -o SHA256SUMS.txt "https://github.com/hknrslnby-eng/je-suis/releases/download/v0.1.0/SHA256SUMS.txt"
sha256sum -c SHA256SUMS.txt --ignore-missing
```

## Sistem Gereksinimleri

| Platform | Gereksinim |
| --- | --- |
| Windows | Windows 10 veya üzeri, 64-bit |
| Linux | Modern 64-bit dağıtım, WebKitGTK uyumlu masaüstü ortamı |
| macOS | Güncel desteklenen macOS sürümü (Intel ve Apple Silicon) |

## Lisans

JeSuis **açık kaynak değildir**. MIT, GPL veya benzeri açık kaynak lisansları bu dağıtım için uygun değildir.

Bu sürüm, **ücretsiz bireysel mesleki kullanım** için sunulur. Kaynak kod verilmez; yeniden dağıtım, tersine mühendislik ve ticari kullanım izin gerektirir. Tüm haklar geliştiricide saklıdır.

Tam metin: [LICENSE.md](LICENSE.md)

**Özet:**

- Ücretsiz indirip kendi mesleki çalışmanızda kullanabilirsiniz.
- Kurulum dosyalarını başkalarına dağıtamaz veya satamazsınız.
- Kaynak kod talep edilemez; gelecekteki ticari lisanslar ayrıca duyurulabilir.

## Sürüm

Güncel sürüm dosyaları bu reponun GitHub Releases bölümünde yayımlanır:

https://github.com/hknrslnby-eng/je-suis/releases

## Destek

Kurulum veya çalıştırma sırasında sorun yaşarsanız, indirdiğiniz dosyanın işletim sisteminize uygun olduğundan ve en güncel release sürümünü kullandığınızdan emin olun. Teknik destek ve lisans talepleri için [Issues](https://github.com/hknrslnby-eng/je-suis/issues) bölümünü kullanabilirsiniz.
