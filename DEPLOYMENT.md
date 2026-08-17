# Teknoloji Rehberleri Web Sitesi

Bu depo, Markdown formatındaki teknoloji rehberlerini GitHub Pages üzerinde yayınlamak için MkDocs kullanır.

## 🚀 Yayına Alma Adımları

### 1. Depoyu GitHub'a Push Edin

```bash
git add .
git commit -m "Web sitesi yapılandırması eklendi"
git push origin main
```

### 2. GitHub Actions'ı Bekleyin

- Depoyu push ettikten sonra GitHub Actions otomatik olarak siteyi derleyip `gh-pages` branch'ine yayınlayacak.
- **Actions** sekmesinden deploy işleminin tamamlanmasını bekleyin.

### 3. GitHub Pages'i Aktif Edin

1. GitHub deposunda **Settings** > **Pages** bölümüne gidin
2. **Source** kısmında:
   - Branch: `gh-pages`
   - Folder: `/ (root)` seçin
3. **Save** butonuna tıklayın

### 4. Sitenize Erişin

Birkaç dakika içinde siteniz şu adreste yayında olacak:
```
https://KULLANICI_ADI.github.io/DEPO_ADI
```

## 📁 Oluşturulan Dosyalar

- `mkdocs.yml`: Site yapılandırması
- `docs/index.md`: Ana sayfa
- `.github/workflows/deploy.yml`: Otomatik deploy iş akışı
- `site/`: Derlenmiş statik dosyalar (lokal test için)

## 🔧 Lokal Test

Siteyi lokal bilgisayarınızda test etmek için:

```bash
pip install mkdocs mkdocs-material
mkdocs serve
```

Tarayıcınızda `http://127.0.0.1:8000` adresini ziyaret edin.

## 🎨 Özellikler

- ✅ Responsive tasarım
- ✅ Koyu/Açık mod desteği
- ✅ Türkçe dil desteği
- ✅ Arama özelliği
- ✅ Kod bloklarında kopyalama butonu
- ✅ Kategorize edilmiş navigasyon

## 📝 İçerik Güncelleme

Herhangi bir rehberi güncellediğinizde, GitHub Actions otomatik olarak siteyi yeniden derleyip yayınlayacaktır.
