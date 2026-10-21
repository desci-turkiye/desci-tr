# desci.tr

DeSci Türkiye topluluğunun web sitesi. Yayın adresi: https://desci.tr

## Yapı

- `index.html`: Sitenin tamamı (içerik, stil ve script tek dosyada). Türkçe ve İngilizce metinler yan yana durur: `data-tr` ve `data-en` öznitelikleriyle işaretlenir, dil düğmesi hangisinin görüneceğini seçer.
- `img/`: Etkinlik fotoğrafları ve favicon.

Derleme adımı yoktur. Vercel, `main` dalına gönderilen her değişikliği otomatik olarak yayına alır.

## İçerik güncelleme

- **Yeni etkinlik:** `index.html` içinde `<section id="events">` altına yeni bir `<article class="ev">` ekleyin. Görseli `img/` klasörüne koyun (genişliği en fazla 1400 px, JPEG).
- **Blog:** `<section id="blog">` altındaki `<article class="post">` kartları.
- Her metni iki dilde yazın: biri `data-tr`, biri `data-en` ile.

## Form

Katılım formu Google Forms'a gönderilecek şekilde hazırlandı. `index.html` içindeki `FORM_URL` ve `FIELDS` değerleri form oluşturulunca doldurulacak. Depoya kişisel veri, şifre ya da API anahtarı eklenmemelidir.
