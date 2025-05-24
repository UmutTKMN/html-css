# HTML & CSS: Sıfırdan

## 🎯 Genel Bakış

HTML ve CSS, web geliştirme dünyasının temel taşlarıdır. Bu rehber, sıfırdan başlayıp profesyonel seviyeye ulaşmak isteyenler için adım adım, uygulamalı ve örneklerle dolu bir yol haritası sunar.

---

## 📚 Temel Kaynaklar

### Türkçe Kaynaklar

- **YouTube Kanalları:**
  - Engin Demirok – HTML/CSS Eğitim Serisi
  - Yazılım Bilimi – Web Geliştirme
  - Geleceği Yazanlar – Frontend Eğitimleri
  - Kablosuz Kedi – Web Tasarım

### İngilizce Kaynaklar

- [MDN Web Docs](https://developer.mozilla.org/) – En kapsamlı dokümantasyon
- [W3Schools](https://www.w3schools.com/) – Başlangıç dostu
- [CSS-Tricks](https://css-tricks.com/) – CSS ipuçları ve rehberler
- [freeCodeCamp](https://www.freecodecamp.org/) – Ücretsiz interaktif kurslar

### Kitaplar

- "HTML5 ve CSS3 ile Web Tasarımı" – Kodlab Yayınları
- "CSS: The Definitive Guide" – Eric Meyer

---

## 🚀 Aşama 1: HTML Temelleri (2-3 Hafta)

### 1.1 HTML'e Giriş

#### HTML Nedir?

HTML (HyperText Markup Language), web sayfalarının temel yapı taşını oluşturan işaretleme dilidir. Web tarayıcıları, HTML dosyalarını okuyarak metin, görsel, bağlantı ve diğer içerikleri kullanıcıya görsel olarak sunar. HTML, "etiketler" (tags) ile çalışır ve her etiket belirli bir işlevi yerine getirir.

#### Web Tarayıcıları ve HTML

Bir HTML dosyası, Chrome, Firefox, Edge gibi tarayıcılarda açıldığında tarayıcı bu dosyayı işler ve kullanıcıya görsel bir arayüz sunar. Tarayıcılar, HTML etiketlerini yorumlayarak metinleri başlık, paragraf, liste, bağlantı gibi farklı biçimlerde gösterir.

#### Temel HTML Belge Yapısı

Bir HTML dosyası, belirli bir iskelet yapısına sahiptir. Bu yapı, tarayıcının sayfanın içeriğini doğru şekilde yorumlamasını sağlar.

```html
<!DOCTYPE html>
<html lang="tr">
  <head>
    <meta charset="UTF-8" />
    <title>Sayfa Başlığı</title>
  </head>
  <body>
    <!-- Sayfa içeriği buraya yazılır -->
  </body>
</html>
```

- `<!DOCTYPE html>`: Dosyanın bir HTML5 belgesi olduğunu belirtir.
- `<html lang="tr">`: Tüm sayfa içeriğini kapsar ve dil bilgisini belirtir.
- `<head>`: Sayfa başlığı, karakter seti, stil dosyaları gibi meta bilgileri içerir.
- `<title>`: Tarayıcı sekmesinde görünen başlık.
- `<body>`: Kullanıcıya gösterilecek asıl içerik burada yer alır.

#### HTML Dosyası Nasıl Oluşturulur?

1. Bir metin editörü (VS Code, Notepad++, Sublime Text vb.) açın.
2. Yukarıdaki temel HTML şablonunu kopyalayın.
3. Dosyayı `index.html` adıyla kaydedin.
4. Dosyayı çift tıklayarak veya tarayıcıda açarak görüntüleyin.

#### Pratik: İlk HTML Sayfanı Oluştur

1. Aşağıdaki kodu bir dosyaya yapıştırın:

```html
<!DOCTYPE html>
<html lang="tr">
  <head>
    <meta charset="UTF-8" />
    <title>Benim İlk Web Sayfam</title>
  </head>
  <body>
    <h1>Merhaba Dünya!</h1>
    <p>Bu benim ilk HTML sayfam.</p>
  </body>
</html>
```

2. Dosyayı kaydedin ve tarayıcıda açın. "Merhaba Dünya!" başlığını ve altındaki paragrafı göreceksiniz.

#### İpuçları

- HTML dosya uzantısı `.html` olmalıdır.
- Türkçe karakterler için `<meta charset="UTF-8">` kullanmak önemlidir.
- Her açılan etiketin (`<html>`, `<head>`, `<body>`) mutlaka kapanışı (`</html>`, `</head>`, `</body>`) olmalıdır.
- Yorum eklemek için `<!-- Yorum buraya -->` kullanılır.

---

### 1.2 Temel HTML Etiketleri

HTML, içerikleri yapılandırmak için birçok farklı etiket sunar. Temel etiketleri ve kullanım amaçlarını aşağıda bulabilirsiniz:

#### 1. Başlık Etiketleri (`<h1>` - `<h6>`)

- Web sayfasındaki başlıkları ve alt başlıkları tanımlar.
- `<h1>` en önemli başlıktır, `<h6>` en düşük seviyededir.

```html
<h1>En Büyük Başlık</h1>
<h2>Alt Başlık</h2>
<h3>Daha Alt Başlık</h3>
```

#### 2. Paragraf Etiketi (`<p>`)

- Metin paragraflarını tanımlar.

```html
<p>Bu bir paragraf örneğidir.</p>
```

#### 3. Bağlantı Etiketi (`<a>`)

- Başka bir sayfaya veya adrese bağlantı verir.

```html
<a href="https://www.ornek.com">Web Sitesine Git</a>
```

#### 4. Görsel Etiketi (`<img>`)

- Sayfaya resim ekler.
- `src` ile resim yolu, `alt` ile açıklama girilir.

```html
<img src="resim.jpg" alt="Açıklama metni" />
```

#### 5. Liste Etiketleri

- **Sırasız Liste (`<ul>`, `<li>`)**

```html
<ul>
  <li>Öğe 1</li>
  <li>Öğe 2</li>
</ul>
```

- **Sıralı Liste (`<ol>`, `<li>`)**

```html
<ol>
  <li>Birinci</li>
  <li>İkinci</li>
</ol>
```

#### 6. Satır İçi ve Blok Etiketler

- **Blok Etiket:** `<div>` (bölümleme için kullanılır)
- **Satır İçi Etiket:** `<span>` (küçük metin parçalarını işaretlemek için)

```html
<div>Bu bir blok etikettir.</div>
<span>Bu bir satır içi etikettir.</span>
```

#### 7. Yorum Satırı

- Kodun içine açıklama eklemek için kullanılır, tarayıcıda görünmez.

```html
<!-- Bu bir HTML yorumudur -->
```

#### 8. Diğer Temel Etiketler

- **Yatay Çizgi:** `<hr>`
- **Satır Sonu:** `<br>`

```html
<p>Birinci satır<br />İkinci satır</p>
<hr />
```

> **Not:** Tüm HTML etiketlerinin açılış ve kapanış etiketleri olmalıdır. Kendi kendine kapanan etiketler: `<img>`, `<br>`, `<hr>` gibi.

---

### 1.3 Metin Biçimlendirme

HTML'de metinleri vurgulamak, öne çıkarmak veya farklı biçimlerde göstermek için çeşitli etiketler kullanılır:

- **Kalın Metin (`<strong>`):** Önemli metinleri kalın gösterir.
  ```html
  <strong>Bu metin kalın ve vurguludur.</strong>
  ```
- **Vurgulu Metin (`<em>`):** Metni italik ve vurgulu gösterir.
  ```html
  <em>Bu metin vurguludur.</em>
  ```
- **İşaretli Metin (`<mark>`):** Metni fosforlu kalemle işaretlenmiş gibi gösterir.
  ```html
  <mark>Bu metin işaretli.</mark>
  ```
- **Satır İçi (`<span>`):** Küçük metin parçalarını işaretlemek için kullanılır.
  ```html
  <span style="color: red;">Kırmızı metin</span>
  ```
- **Blok (`<div>`):** Birden fazla öğeyi veya bölümü gruplamak için kullanılır.
  ```html
  <div>Bu bir blok bölümdür.</div>
  ```
- **Satır Kesme (`<br>`):** Satır sonu ekler.
  ```html
  Birinci satır<br />İkinci satır
  ```
- **Yatay Çizgi (`<hr>`):** Sayfa içinde yatay bir ayraç çizer.
  ```html
  <hr />
  ```

---

### 1.4 HTML Formları

Formlar, kullanıcıdan veri almak için kullanılır. Temel form elemanları şunlardır:

- **Form Kapsayıcısı (`<form>`):** Tüm form elemanlarını kapsar.
- **Giriş Alanı (`<input>`):** Tek satırlık veri girişi sağlar.
- **Çok Satırlı Alan (`<textarea>`):** Uzun metinler için kullanılır.
- **Açılır Menü (`<select>`, `<option>`):** Seçim listesi sunar.
- **Buton (`<button>`):** Formu göndermek veya işlem yapmak için kullanılır.

Örnek form:

```html
<form>
  <input type="text" placeholder="Adınız" required />
  <input type="email" placeholder="E-posta" />
  <textarea placeholder="Mesajınız"></textarea>
  <select>
    <option>Seçenek 1</option>
    <option>Seçenek 2</option>
  </select>
  <button type="submit">Gönder</button>
</form>
```

- **Doğrulama:**
  - `required`: Boş bırakılamaz.
  - `type="email"`: E-posta formatı kontrolü.
  - `pattern`: Düzenli ifade ile özel kontrol.

---

### 1.5 Semantic HTML

Semantic HTML, sayfa yapısını ve içeriğin anlamını daha iyi ifade eden etiketler kullanmayı amaçlar. Bu, hem SEO hem de erişilebilirlik için önemlidir.

- **Yapısal Etiketler:**
  - `<header>`: Sayfa veya bölüm başlığı
  - `<nav>`: Navigasyon menüsü
  - `<main>`: Ana içerik
  - `<section>`: Mantıksal bölüm
  - `<article>`: Bağımsız içerik (ör. blog yazısı)
  - `<aside>`: Yan içerik veya ek bilgi
  - `<footer>`: Alt bilgi

Örnek yapı:

```html
<header>
  <h1>Site Başlığı</h1>
  <nav>
    <a href="#">Anasayfa</a>
    <a href="#">Hakkında</a>
  </nav>
</header>
<main>
  <section>
    <h2>Bölüm Başlığı</h2>
    <p>Bölüm içeriği...</p>
  </section>
  <article>
    <h2>Blog Yazısı</h2>
    <p>Yazı içeriği...</p>
  </article>
  <aside>
    <p>Ek bilgi veya reklam</p>
  </aside>
</main>
<footer>
  <p>© 2025 Tüm hakları saklıdır.</p>
</footer>
```

---

### 1.6 Pratik Projeler

#### 1. Kişisel CV Sayfası

- **Amaç:** Temel HTML etiketleriyle kişisel bilgiler, eğitim ve deneyim bölümleri oluşturun.
- **İçerik:**
  - Ad, iletişim bilgileri
  - Eğitim geçmişi (liste)
  - İş deneyimi (başlık ve paragraflar)
  - Yetenekler (liste)

#### 2. Basit Blog Yazısı

- **Amaç:** Semantic HTML kullanarak bir blog yazısı şablonu hazırlayın.
- **İçerik:**
  - `<article>` ile ana yazı
  - `<header>` ile başlık ve yazar bilgisi
  - `<img>` ile görsel
  - `<p>` ile paragraflar

#### 3. İletişim Formu

- **Amaç:** Ad, e-posta ve mesaj alanları içeren bir form tasarlayın.
- **İçerik:**
  - `<form>`, `<input>`, `<textarea>`, `<button>`
  - Doğrulama için `required` ve `type="email"` kullanımı

Her proje için kodunuzu yazıp tarayıcıda test edin. Geliştirdikçe yeni özellikler ekleyin (ör. sosyal medya linkleri, stil ekleme, ek alanlar).

---

## 🎨 Aşama 2: CSS Temelleri (3-4 Hafta)

### 2.1 CSS'e Giriş

CSS (Cascading Style Sheets), HTML ile oluşturulan web sayfalarının görsel tasarımını ve düzenini belirlemek için kullanılır. HTML yapıyı, CSS ise görünümü sağlar.

#### CSS Ekleme Yöntemleri

- **Inline CSS:** Etiketin `style` özelliği ile doğrudan uygulanır.
  ```html
  <p style="color: red;">Kırmızı metin</p>
  ```
- **Internal CSS:** `<style>` etiketi ile HTML dosyasının `<head>` bölümünde tanımlanır.
  ```html
  <style>
    p {
      color: red;
    }
  </style>
  ```
- **External CSS (Önerilen):** Ayrı bir `.css` dosyası oluşturulup `<link>` etiketiyle bağlanır.
  ```html
  <link rel="stylesheet" href="style.css" />
  ```

---

### 2.2 Temel CSS Özellikleri

CSS ile renk, yazı tipi, kenarlık, boşluk gibi birçok görsel özellik kontrol edilir.

- **Renkler:**
  ```css
  .renkli {
    color: #3498db;
    background-color: #f1f1f1;
  }
  ```
- **Yazı Tipleri:**
  ```css
  .yazi {
    font-family: Arial, sans-serif;
    font-size: 18px;
    font-weight: bold;
  }
  ```
- **Metin Hizalama:**
  ```css
  .ortala {
    text-align: center;
    line-height: 1.5;
  }
  ```
- **Kenarlıklar:**
  ```css
  .kutu {
    border: 2px solid #333;
    border-radius: 8px;
  }
  ```
- **Boşluklar:**
  ```css
  .bosluk {
    margin: 20px;
    padding: 10px;
  }
  ```

---

### 2.3 CSS Box Model

Box Model, her HTML öğesinin bir kutu (box) olarak ele alınmasını sağlar. Bu kutu dört ana bölümden oluşur:

- **Content:** İçerik alanı
- **Padding:** İçerik ile kenarlık arasındaki boşluk
- **Border:** Kenarlık
- **Margin:** Dış boşluk

```css
.box {
  width: 200px;
  height: 100px;
  padding: 20px;
  border: 2px solid #333;
  margin: 10px;
}
```

- **Box Sizing:**
  ```css
  * {
    box-sizing: border-box;
  }
  ```
  Bu özellik, padding ve border'ın toplam genişlik ve yüksekliğe dahil edilmesini sağlar.

---

### 2.4 CSS Seçiciler

Seçiciler, hangi HTML elemanına stil uygulanacağını belirler.

- **Element Seçici:**
  ```css
  p {
    color: blue;
  }
  ```
- **Class Seçici:**
  ```css
  .kirmizi {
    color: red;
  }
  ```
- **ID Seçici:**
  ```css
  #ozel {
    font-size: 24px;
  }
  ```
- **Pseudo-class:**
  ```css
  a:hover {
    color: green;
  }
  input:focus {
    border-color: blue;
  }
  ```
- **Kombinasyon Seçiciler:**
  ```css
  div > p {
    color: orange;
  }
  ul li {
    font-weight: bold;
  }
  h1 + p {
    margin-top: 0;
  }
  ```

---

### 2.5 Pozisyonlama

CSS ile bir öğenin sayfadaki konumu farklı şekillerde ayarlanabilir:

- **Position Değerleri:**

  - `static`: Varsayılan konumlandırma
  - `relative`: Kendi normal konumuna göre
  - `absolute`: En yakın konumlandırılmış üst elemana göre
  - `fixed`: Ekrana sabitlenir
  - `sticky`: Kaydırmaya göre sabitlenir

  ```css
  .sabit {
    position: fixed;
    top: 0;
    left: 0;
  }
  .goreceli {
    position: relative;
    left: 20px;
  }
  ```

- **Z-index:** Katman sıralaması için kullanılır.
  ```css
  .ustte {
    z-index: 10;
  }
  ```

---

### 2.6 Pratik Projeler

- **HTML Sayfalarını Güzelleştirme:**
  - Renk, yazı tipi, boşluk ve kenarlıklarla sayfanızı stilize edin.
- **Basit Kart Tasarımları:**
  - Modern kart bileşenleri oluşturun. Örneğin ürün veya profil kartı.
- **Navigation Bar:**
  - Flexbox ile responsive menü tasarlayın. Menüde hover efektleri ve aktif durumlar ekleyin.

Her projede CSS dosyanızı HTML'e bağlamayı ve farklı stiller denemeyi unutmayın.

---

## 📱 Aşama 3: Responsive Tasarım (2-3 Hafta)

### 3.1 Flexbox

- **Kapsayıcı:**  
  `display: flex;`, `flex-direction`, `justify-content`, `align-items`
- **Örnek:**

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

---

### 3.2 CSS Grid

- **Kapsayıcı:**  
  `display: grid;`, `grid-template-columns`, `grid-gap`
- **Örnek:**

```css
.grid {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  gap: 20px;
}
```

---

### 3.3 Media Queries

- **Temel Kullanım:**

```css
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

- **Breakpoint Önerileri:**
  - 576px: Telefon
  - 768px: Tablet
  - 992px: Küçük masaüstü
  - 1200px: Büyük masaüstü

---

### 3.4 Modern CSS Units

- **rem, em:**  
  Yazı ve boşluklarda ölçeklenebilirlik
- **vw, vh:**  
  Ekran boyutuna göre oranlama
- **fr:**  
  Grid için esnek oran

---

### 3.5 Pratik Projeler

- **Responsive Kart Galeri:**  
  Grid ve media queries ile farklı ekranlarda uyumlu kartlar.
- **Mobile-Friendly Navigation:**  
  Hamburger menü ve responsive navbar.
- **Responsive Blog Layout:**  
  Grid ve flexbox kombinasyonu ile modern blog şablonu.

---

## 🚀 Aşama 4: İleri Seviye CSS (3-4 Hafta)

### 4.1 CSS Animations ve Transitions

Animasyonlar ve geçişler, web sitenize hareket ve etkileşim kazandırır.

#### CSS Transitions

- Bir özelliğin bir durumdan diğerine yumuşak geçişini sağlar.
- Sık kullanılan özellikler: `transition-property`, `transition-duration`, `transition-timing-function`, `transition-delay`

```css
.button {
  background: #3498db;
  color: #fff;
  transition: background 0.3s, transform 0.2s;
}
.button:hover {
  background: #2ecc71;
  transform: scale(1.05);
}
```

#### CSS Animations

- Daha karmaşık hareketler için `@keyframes` ile tanımlanır.

```css
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
.box {
  animation: fadeIn 1s ease-in;
}
```

- Özellikler: `animation-name`, `animation-duration`, `animation-timing-function`, `animation-delay`, `animation-iteration-count`, `animation-direction`

---

### 4.2 CSS Preprocessors (Sass/SCSS)

CSS ön işlemciler, daha okunabilir ve yönetilebilir stil dosyaları yazmanızı sağlar.

- **Değişkenler:** Tek bir yerde tanımlanıp her yerde kullanılabilir.
- **Nesting:** Seçicileri iç içe yazma imkanı.
- **Mixin:** Tekrarlayan kodları fonksiyon gibi kullanma.

```scss
$primary: #3498db;
@mixin button($bg, $color) {
  background: $bg;
  color: $color;
  border-radius: 4px;
}
.button {
  @include button($primary, #fff);
}
```

---

### 4.3 CSS Metodolojileri

Büyük projelerde CSS kodlarının okunabilir, sürdürülebilir ve yönetilebilir olması için çeşitli metodolojiler kullanılır. En yaygınlarından biri BEM'dir.

#### BEM (Block Element Modifier)

- **Amaç:** Sınıf isimlendirmesini standartlaştırmak ve stil çakışmalarını önlemek.
- **Yapı:**
  - **Block:** Bağımsız bileşen (ör: `card`)
  - **Element:** Blok içindeki alt parça (ör: `card__title`)
  - **Modifier:** Blok veya elementin varyasyonu (ör: `card__button--primary`)

```html
<div class="card">
  <h2 class="card__title">Başlık</h2>
  <button class="card__button card__button--primary">Buton</button>
</div>
```

- **Diğer Metodolojiler:**
  - OOCSS (Object Oriented CSS)
  - SMACSS (Scalable and Modular Architecture for CSS)
  - Atomic CSS

Her projede tutarlı bir metodoloji kullanmak, kodunuzu büyüdükçe daha kolay yönetmenizi sağlar.

---

## 📈 İlerleme Takibi

Başarılı bir öğrenme süreci için ilerlemenizi haftalık ve proje bazlı olarak takip edin.

### Haftalık Hedefler

- **1-2. Hafta:** HTML temelleri, basit sayfalar
- **3-4. Hafta:** CSS temelleri, styling
- **5-6. Hafta:** Layout ve positioning
- **7-8. Hafta:** Responsive design
- **9-10. Hafta:** Animasyonlar ve ileri CSS
- **11-12. Hafta:** Proje geliştirme

### Milestone Projeleri

1. **Kişisel Portföy Sitesi** (HTML + CSS)
2. **Responsive E-ticaret Ürün Sayfası**
3. **Modern Blog Template**
4. **Landing Page with Animations**

Her aşamadan sonra kendi projenizi geliştirerek öğrendiklerinizi pekiştirin.

---

## 🎯 Önemli İpuçları

- **Düzenli pratik yapın:** Her gün kısa süreli de olsa kod yazın.
- **Kod yazarak öğrenin:** Sadece okumak yerine uygulayarak öğrenin.
- **Projeler geliştirin:** Gerçek projelerle bilgilerinizi pekiştirin.
- **Topluluklara katılın:** Stack Overflow, Reddit gibi platformlarda soru sorun, cevap verin.
- **Farklı cihazlarda test edin:** Mobil ve masaüstü uyumluluğunu kontrol edin.
- **Developer Tools kullanın:** Tarayıcıların geliştirici araçlarını aktif kullanın.
- **Kodunuzu düzenli ve okunabilir tutun.**

---

## 🔗 Faydalı Linkler

### Dokumentasyon

- [MDN HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [MDN CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3Schools](https://www.w3schools.com/)

### Pratik ve Proje Siteleri

- [freeCodeCamp](https://www.freecodecamp.org/)
- [Codecademy](https://www.codecademy.com/)
- [Frontend Mentor](https://www.frontendmentor.io/)

### Tasarım ve İlham

- [Dribbble](https://dribbble.com/)
- [Behance](https://www.behance.net/)
- [Awwwards](https://www.awwwards.com/)

### CSS Araçları

- [CSS Grid Generator](https://grid.layoutit.com/)
- [Flexbox Generator](https://flexbox.help/)
- [Box Shadow Generator](https://box-shadow.dev/)

---

## 🎉 Sonuç

Bu yol haritasını takip ederek 3-6 ay içinde HTML ve CSS konularında yetkin hale gelebilirsiniz. Unutmayın ki en önemli şey **düzenli pratik yapmak** ve **projeler geliştirmek**tir. Kod yazmaya başlayın ve öğrendiklerinizi hemen uygulayın!

**Başarılar! 🚀**

---
