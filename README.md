# HTML Açıklama Üretici

Ticimax (ve benzeri e-ticaret altyapıları) için **toplu ürün açıklaması HTML'i** üreten, tek dosyalık, tarayıcıda çalışan bir araç. Excel dosyanızı yükler, sütunları eşleştirir, her ürüne özel HTML açıklama sütunu eklenmiş yeni bir Excel indirir.

Tüm işlem tarayıcıda gerçekleşir — **hiçbir veri internete gönderilmez.**

## Özellikler

- **Excel / CSV okuma** — `.xlsx`, `.xls`, `.csv` desteği, çoklu sayfa seçimi
- **Sütun eşleştirme** — başlık sütunu seçimi, "Etiket + Sütun" mantığıyla teknik özellikler tablosu kurma, satır sıralama
- **Akıllı tahmin** — diş, genişlik, profil gibi teknik sütunları otomatik tanıyıp tabloya ekler
- **Yer tutucular** — giriş paragrafı ve ek HTML alanında `{Sütun Adı}` ile herhangi bir sütun değeri kullanılabilir
- **Düzenlenebilir önizleme** — render edilmiş görünümün üzerine tıklayıp ürüne özel düzenleme yapın; düzenlemeler Excel çıktısına yansır
- **Boş değer temizliği** — değeri boş olan özellik satırları tablodan otomatik çıkarılır
- **Excel sınır koruması** — 32.767 karakter hücre sınırını aşan içerikler kırpılır ve satır/sütun bazında raporlanır
- **HTML sıkıştırma** — gereksiz boşluklar silinerek karakter tasarrufu sağlanır

## Kullanım

1. `index.html` dosyasını tarayıcıda açın (çift tıklamak yeterli)
2. Ürün Excel'inizi yükleyin
3. Başlık sütununu ve teknik özellik eşleştirmelerini yapın
4. Önizlemede ürünler arasında gezip kontrol edin
5. "Tüm ürünlere uygula ve Excel indir" — çıkan dosyayı Ticimax'a toplu yükleyin

> Çıktı sütununun adını Ticimax içe aktarma şablonunuzdaki başlıkla birebir aynı yaparsanız dosyayı doğrudan yükleyebilirsiniz.

## Online yayınlama (opsiyonel)

- **Netlify:** [app.netlify.com/drop](https://app.netlify.com/drop) sayfasına bu klasörü sürükleyin
- **Vercel:** `vercel` komutunu klasör içinde çalıştırın
- **GitHub Pages:** Repoyu GitHub'a gönderin, Settings → Pages → kaynak olarak `main` seçin

## GitHub'a gönderme

```bash
cd "HTML-Aciklama-Uretici"
git remote add origin https://github.com/KULLANICI_ADINIZ/html-aciklama-uretici.git
git push -u origin main
```

## Teknolojiler

- Saf HTML / CSS / JavaScript — derleme adımı yok
- [SheetJS (xlsx)](https://sheetjs.com/) — CDN üzerinden, Excel okuma/yazma

## Lisans

MIT
