# JeSuis

JeSuis; hukuk, arabuluculuk, dosya, gider, makbuz ve çalışma alanı süreçlerini tek masaüstü uygulamasında toplamak için hazırlanmış profesyonel bir iş takip uygulamasıdır.

Bu repo yalnızca son kullanıcı dağıtım dosyalarını içerir. Kaynak kod, geliştirme dosyaları ve özel yapılandırmalar bu repoda yayımlanmaz.

**Güncel sürüm:** [v0.1.0](https://github.com/hknrslnby-eng/je-suis/releases/tag/v0.1.0)

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

## Sürüm

Güncel sürüm dosyaları bu reponun GitHub Releases bölümünde yayımlanır:

https://github.com/hknrslnby-eng/je-suis/releases

## Destek

Kurulum veya çalıştırma sırasında sorun yaşarsanız, indirdiğiniz dosyanın işletim sisteminize uygun olduğundan ve en güncel release sürümünü kullandığınızdan emin olun.
