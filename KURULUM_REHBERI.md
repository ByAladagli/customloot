# CustomLoot Pro - Kurulum ve Yayınlama Rehberi

## 🚀 Hızlı Başlangıç (3 Dakikada)

### Adım 1: Dosyaları İndirin
Claude'dan aldığınız bu dosyaları bilgisayarınıza indirin:
- ✅ `customloot-pro-tr-updated.html` - Ana uygulama
- ✅ `rust-items-complete.json` - Eşya veritabanı

### Adım 2: Hemen Kullanmaya Başlayın
1. `customloot-pro-tr-updated.html` dosyasına **çift tıklayın**
2. Tarayıcınızda (Chrome, Firefox, Edge) otomatik açılacak
3. Hepsi bu kadar! ✨

**Not:** İnternet bağlantısı gerekmez, tamamen offline çalışır!

---

## 💻 Yerel Kullanım (Kendi Bilgisayarınızda)

### Yöntem 1: Tarayıcıda Direkt Açma (EN KOLAY)
```
1. HTML dosyasına çift tıklayın
2. Ya da sağ tık → "Birlikte Aç" → Tarayıcı seçin
3. Kullanmaya başlayın!
```

**Avantajlar:**
- ✅ Kurulum gerektirmez
- ✅ Anında çalışır
- ✅ Tüm özellikler çalışır

### Yöntem 2: Yerel Sunucu ile Çalıştırma (Önerilen)

#### Python ile (Kolay)
```bash
# Python 3 kurulu mu kontrol edin
python --version

# Dosyanın bulunduğu klasöre gidin
cd /dosyanın/olduğu/klasör

# Sunucuyu başlatın
python -m http.server 8000

# Tarayıcıda açın:
# http://localhost:8000/customloot-pro-tr-updated.html
```

#### Node.js ile
```bash
# http-server yükleyin (bir kez)
npm install -g http-server

# Sunucuyu başlatın
http-server -p 8000

# Tarayıcıda açın:
# http://localhost:8000/customloot-pro-tr-updated.html
```

#### VS Code ile
```
1. VS Code'u açın
2. Dosyayı açın
3. Sağ tık → "Open with Live Server"
```

---

## 🌐 Web'de Yayınlama (Herkes Erişebilir)

### Seçenek 1: GitHub Pages (ÜCRETSİZ & Kolay)

#### Adım Adım:
```bash
1. GitHub'da yeni bir repository oluşturun
   - Adı: customloot-pro
   - Public seçin

2. Dosyaları yükleyin:
   git init
   git add customloot-pro-tr-updated.html
   git add rust-items-complete.json
   git commit -m "CustomLoot Pro eklendi"
   git branch -M main
   git remote add origin https://github.com/KULLANICI_ADI/customloot-pro.git
   git push -u origin main

3. Settings → Pages bölümüne gidin
   - Source: main branch
   - Kaydet

4. 5 dakika içinde yayında!
   URL: https://KULLANICI_ADI.github.io/customloot-pro/customloot-pro-tr-updated.html
```

**Avantajlar:**
- ✅ Tamamen ücretsiz
- ✅ HTTPS desteği
- ✅ Hızlı ve güvenilir
- ✅ Otomatik güncellemeler

### Seçenek 2: Netlify (ÜCRETSİZ & Çok Kolay)

#### Drag & Drop ile:
```
1. https://app.netlify.com/ adresine gidin
2. "Add new site" → "Deploy manually"
3. HTML dosyasını sürükleyip bırakın
4. 30 saniyede yayında!
```

**Avantajlar:**
- ✅ Git gerekmez
- ✅ Anında deploy
- ✅ Özel domain desteği
- ✅ Otomatik HTTPS

### Seçenek 3: Vercel (ÜCRETSİZ & Profesyonel)

```bash
1. Vercel CLI yükleyin
   npm i -g vercel

2. Deploy edin
   vercel

3. Tamamlandı!
```

### Seçenek 4: Cloudflare Pages (ÜCRETSİZ)

```
1. https://pages.cloudflare.com/ adresine gidin
2. GitHub repo'nuzu bağlayın
3. Deploy edin
4. Hızlı CDN ile dünya çapında erişim!
```

### Seçenek 5: Kendi Sunucunuz

#### Apache ile:
```bash
# Dosyaları web root'a kopyalayın
sudo cp customloot-pro-tr-updated.html /var/www/html/
sudo cp rust-items-complete.json /var/www/html/

# Apache'yi restart edin
sudo systemctl restart apache2

# Erişim: http://sunucu-ip/customloot-pro-tr-updated.html
```

#### Nginx ile:
```bash
# Dosyaları kopyalayın
sudo cp customloot-pro-tr-updated.html /usr/share/nginx/html/
sudo cp rust-items-complete.json /usr/share/nginx/html/

# Nginx'i restart edin
sudo systemctl restart nginx

# Erişim: http://sunucu-ip/customloot-pro-tr-updated.html
```

---

## 🎮 Rust Sunucunuzda Kullanım

### 1. Config Oluşturma
```
1. Web arayüzünü açın
2. Loot tablolarınızı oluşturun
3. NPC ve container ayarlarını yapın
4. "Dışa Aktar" butonuna tıklayın
5. CustomLoot_Config.json indirilir
```

### 2. Sunucuya Yükleme
```bash
# FTP veya SFTP ile bağlanın
# Dosyayı şuraya kopyalayın:
/oxide/config/CustomLoot.json

# Sunucuda reload edin:
rcon "o.reload CustomLoot"
```

### 3. Kontrol
```
1. Sunucuya girin
2. Bir sandık açın veya NPC öldürün
3. Loot'ların değiştiğini görün!
```

---

## 🔧 Özelleştirme

### Dosya Adını Değiştirme
```
customloot-pro-tr-updated.html → index.html

Bu sayede:
https://site.com/index.html yerine
https://site.com/ şeklinde erişebilirsiniz
```

### Özel Domain Bağlama

#### GitHub Pages:
```
1. Repository → Settings → Pages
2. Custom domain: customloot.senindomain.com
3. DNS'te CNAME kaydı ekle
4. Tamamlandı!
```

#### Netlify:
```
1. Site settings → Domain management
2. "Add custom domain"
3. DNS ayarlarını yapın
4. Otomatik SSL aktif olur
```

### Logo ve Renkleri Değiştirme
HTML dosyasını text editör ile açın ve CSS bölümünü düzenleyin:
```css
/* Renkleri değiştirin */
:root {
    --accent-cyan: #58a6ff;  /* Ana renk */
    --accent-purple: #bc8cff; /* İkincil renk */
    --bg-dark: #0d1117;       /* Arka plan */
}
```

---

## 📱 Mobil Uyumluluk

Araç zaten responsive tasarıma sahip:
- ✅ Telefonlarda çalışır
- ✅ Tabletlerde çalışır
- ✅ Touch screen desteği
- ✅ Mobil menüler

---

## 🔒 Güvenlik

### Genel Kullanım İçin:
- ✅ Tamamen güvenli (sadece HTML/CSS/JS)
- ✅ Sunucu tarafı kod yok
- ✅ Veritabanı yok
- ✅ Giriş/kayıt yok

### Özel Kullanım İçin Koruma:

#### Basic Auth (Apache):
```apache
# .htaccess dosyası oluşturun
AuthType Basic
AuthName "CustomLoot Pro"
AuthUserFile /path/to/.htpasswd
Require valid-user
```

```bash
# Şifre oluşturun
htpasswd -c .htpasswd admin
```

#### Basic Auth (Nginx):
```nginx
location /customloot-pro {
    auth_basic "Restricted Access";
    auth_basic_user_file /etc/nginx/.htpasswd;
}
```

---

## 🎓 Video Tutorial Oluşturma

Eğer YouTube'da paylaşmak isterseniz:

### Kayıt Önerileri:
```
1. OBS Studio ile ekranı kaydedin
2. Mikrofon açıklaması ekleyin
3. Adım adım gösterin:
   - Nasıl açılır
   - Nasıl loot table oluşturulur
   - Nasıl export edilir
   - Rust sunucusuna nasıl yüklenir

4. Editleyip yayınlayın!
```

### Örnek Video Yapısı:
```
0:00 - Giriş
0:30 - Kurulum
2:00 - Arayüz tanıtımı
5:00 - Loot table oluşturma
8:00 - Export ve Rust'a yükleme
10:00 - Test ve sonuç
```

---

## 🌟 Toplulukla Paylaşma

### Discord'da:
```
1. Rust sunucu Discord'unuzda paylaşın
2. #tools veya #resources kanalında
3. Link ve kısa açıklama paylaşın
```

### Reddit'te:
```
r/playrust
r/playrustadmin
r/RustConsole

Başlık: "CustomLoot Pro - Free GUI Tool for Server Admins"
```

### Rust Forums:
```
https://forum.facepunch.com/
- Server Administration bölümünde
```

---

## ❓ Sık Sorulan Sorular

### S: İnternet gerekli mi?
**C:** Hayır! Tamamen offline çalışır. Sadece Google Fonts için internet gerekir (opsiyonel).

### S: Hangi tarayıcılar destekleniyor?
**C:** 
- ✅ Chrome/Edge (Önerilen)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

### S: Mobilde çalışır mı?
**C:** Evet! Responsive tasarım sayesinde mobilde de çalışır.

### S: Verilerim kaybolur mu?
**C:** Browser localStorage kullanılmıyor, her zaman export edip kaydedin!

### S: Ücretsiz mi?
**C:** Evet, tamamen ücretsiz ve açık kaynak!

### S: Nasıl güncelleme alırım?
**C:** Yeni HTML dosyasını indirip eskisinin yerine koyun.

### S: Özelleştirme yapabilir miyim?
**C:** Evet! HTML/CSS/JS dosyası açık, istediğiniz gibi düzenleyebilirsiniz.

### S: Başka dillere çevirebilir miyim?
**C:** Evet! HTML dosyasındaki text'leri değiştirin.

---

## 🛠️ Teknik Destek

### Hata Bulursanız:
```
1. Tarayıcı Console'u açın (F12)
2. Hata mesajını kopyalayın
3. GitHub Issues'da bildirin
   VEYA
4. Discord/Forum'da paylaşın
```

### Özellik İsteği:
```
1. GitHub'da Issue açın
2. Detaylı açıklama yapın
3. Örnek görseller ekleyin
```

---

## 📊 İstatistikler (Opsiyonel)

### Google Analytics Ekleme:
```html
<!-- HEAD bölümüne ekleyin -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🎉 Başarı Hikayeleri

Aracı kullanıp paylaşırsanız:
- ⭐ GitHub'da star verin
- 📢 Sosyal medyada paylaşın
- 💬 Geri bildirimde bulunun
- 🤝 Toplulukla paylaşın

---

## 📞 İletişim ve Destek

### GitHub:
```
https://github.com/KULLANICI_ADI/customloot-pro
- Issues: Hata bildirimi
- Discussions: Genel konuşmalar
- Pull Requests: Katkıda bulunma
```

### Discord:
```
Rust Admin/Server Discord'larında
#admin-tools veya #resources kanallarında
```

---

## 🔥 Hızlı Deploy Komutları

### Netlify (En Hızlı):
```bash
# Netlify CLI
npm i -g netlify-cli
netlify deploy --prod
```

### Vercel (En Kolay):
```bash
# Vercel CLI
npm i -g vercel
vercel --prod
```

### GitHub Pages (En Popüler):
```bash
git init
git add .
git commit -m "Deploy CustomLoot Pro"
git branch -M main
git remote add origin URL
git push -u origin main
# Settings → Pages → Enable
```

---

## ✅ Kontrol Listesi

Yayınlamadan önce:
- [ ] HTML dosyası test edildi
- [ ] Tüm özellikler çalışıyor
- [ ] Export/Import test edildi
- [ ] Mobil uyumluluk kontrol edildi
- [ ] README dosyası hazırlandı
- [ ] Lisans eklendi (MIT önerilir)
- [ ] GitHub repo oluşturuldu
- [ ] Deploy yapıldı
- [ ] Link test edildi
- [ ] Toplulukla paylaşıldı

---

## 🚀 Hemen Başlayın!

**En basit yol:**
```
1. HTML dosyasına çift tıklayın
2. Kullanmaya başlayın
3. Export edin
4. Rust sunucunuza yükleyin
```

**Yayınlamak için en hızlı yol:**
```
1. GitHub'da repo oluşturun
2. Dosyaları yükleyin
3. Pages'i aktif edin
4. Link'i paylaşın
```

---

## 📚 Ek Kaynaklar

- [Rust Admin Commands](https://www.corrosionhour.com/rust-admin-commands/)
- [Oxide Plugins](https://umod.org/plugins/custom-loot)
- [Rust Wiki](https://rust.fandom.com/wiki/Rust_Wiki)
- [Server Hosting](https://www.gtxgaming.co.uk/rust-server-hosting/)

---

**🎮 Başarılar ve iyi oyunlar! 🎮**

*CustomLoot Pro ile Rust sunucunuzun loot sistemini tam kontrolünüz altına alın!*
