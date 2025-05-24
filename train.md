# HTML & CSS: Sıfırdan Uzmanlığa Detaylı Eğitim

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

- **HTML Nedir?**  
  Web sayfalarının iskeletini oluşturan işaretleme dilidir.
- **Web Tarayıcıları ve HTML**  
  Tarayıcılar, HTML dosyalarını okuyup görsel olarak işler.
- **Temel HTML Belge Yapısı**

```html
<!DOCTYPE html>
<html lang="tr">
  <head>
    <meta charset="UTF-8" />
    <title>Başlık</title>
  </head>
  <body>
    <!-- İçerik buraya -->
  </body>
</html>
```

---

### 1.2 Temel HTML Etiketleri

- **Başlıklar:** `<h1>` - `<h6>`
- **Paragraf:** `<p>`
- **Bağlantı:** `<a href="https://ornek.com">Tıkla</a>`
- **Görsel:** `<img src="resim.jpg" alt="Açıklama">`
- **Liste:**
  - Sırasız: `<ul><li>Öğe</li></ul>`
  - Sıralı: `<ol><li>Öğe</li></ol>`

---

### 1.3 Metin Biçimlendirme

- **Kalın:** `<strong>Kalın</strong>`
- **Vurgulu:** `<em>Vurgulu</em>`
- **İşaretli:** `<mark>Önemli</mark>`
- **Satır içi:** `<span>Metin</span>`
- **Blok:** `<div>Blok</div>`
- **Satır Kesme:** `<br>`
- **Yatay Çizgi:** `<hr>`

---

### 1.4 HTML Formları

- **Form Temelleri:**

```html
<form>
  <input type="text" placeholder="Adınız" required />
  <input type="email" placeholder="E-posta" />
  <textarea placeholder="Mesajınız"></textarea>
  <button type="submit">Gönder</button>
</form>
```

- **Doğrulama:**  
  `required`, `type="email"`, `pattern` gibi özelliklerle form doğrulama yapılır.

---

### 1.5 Semantic HTML

- **Yapısal Etiketler:**

```html
<header>Başlık</header>
<nav>Menü</nav>
<main>
  <section>Bölüm</section>
  <article>Makale</article>
  <aside>Yan Panel</aside>
</main>
<footer>Alt Bilgi</footer>
```

---

### 1.6 Pratik Projeler

- **Kişisel CV Sayfası:**  
  Temel etiketlerle kişisel bilgiler, eğitim ve deneyim bölümleri oluşturun.
- **Basit Blog Yazısı:**  
  `<article>`, `<header>`, `<main>`, `<img>`, `<p>` kullanarak bir blog şablonu hazırlayın.
- **İletişim Formu:**  
  Ad, e-posta ve mesaj alanları içeren bir form tasarlayın.

---

## 🎨 Aşama 2: CSS Temelleri (3-4 Hafta)

### 2.1 CSS'e Giriş

- **CSS Nedir?**  
  Web sayfalarının görsel tasarımını belirler.
- **Ekleme Yöntemleri:**
  - Inline: `<p style="color:red;">Kırmızı</p>`
  - Internal: `<style>p { color: red; }</style>`
  - External: `<link rel="stylesheet" href="style.css">`

---

### 2.2 Temel CSS Özellikleri

- **Renkler:**  
  `color`, `background-color`
- **Yazı Tipleri:**  
  `font-family`, `font-size`, `font-weight`
- **Metin Hizalama:**  
  `text-align`, `line-height`
- **Kenarlıklar:**  
  `border`, `border-radius`
- **Boşluklar:**  
  `margin`, `padding`

```css
.box {
  color: #333;
  background-color: #f9f9f9;
  border: 2px solid #ddd;
  border-radius: 8px;
  padding: 16px;
  margin: 16px 0;
}
```

---

### 2.3 CSS Box Model

- **Bileşenler:**  
  Content, padding, border, margin
- **Box Sizing:**  
  `box-sizing: border-box;` ile toplam genişlik/height kontrolü

---

### 2.4 CSS Seçiciler

- **Element:** `p { ... }`
- **Class:** `.kutu { ... }`
- **ID:** `#ozel { ... }`
- **Pseudo-class:** `a:hover { color: red; }`
- **Kombinasyon:** `div > p`, `ul li`, `h1 + p`

---

### 2.5 Pozisyonlama

- **Position:**  
  `static`, `relative`, `absolute`, `fixed`, `sticky`
- **Z-index:**  
  Katman sıralaması için kullanılır.

---

### 2.6 Pratik Projeler

- **HTML Sayfalarını Güzelleştirme:**  
  Renk, yazı tipi, boşluk ve kenarlıklarla sayfanızı stilize edin.
- **Basit Kart Tasarımları:**  
  Modern kart bileşenleri oluşturun.
- **Navigation Bar:**  
  Flexbox ile responsive menü tasarlayın.

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

- **Transition:**

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

- **Animation:**

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

---

### 4.2 CSS Preprocessors (Sass/SCSS)

- **Değişkenler, Nesting, Mixin:**

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

- **BEM (Block Element Modifier):**

```html
<div class="card">
  <h2 class="card__title">Başlık</h2>
  <button class="card__button card__button--primary">Buton</button>
</div>
```

---

### 4.4 Modern CSS Features

- **CSS Variables:**

```css
:root {
  --main-color: #3498db;
}
.header {
  color: var(--main-color);
}
```

- **Advanced Grid, Subgrid, Container Queries:**  
  Modern tarayıcı desteğiyle gelişmiş layout teknikleri.

---

### 4.5 Pratik Projeler

- **Animasyonlu Landing Page**
- **Etkileşimli Hover Efektleri**
- **Karmaşık Grid Layouts**

---

## 🛠️ Pratik Araçlar

- **Editörler:** VS Code, Sublime Text, Atom
- **VS Code Eklentileri:** Live Server, Emmet, Prettier
- **Online Editörler:** CodePen, JSFiddle, Repl.it
- **Tasarım Araçları:** Figma, Adobe XD, Canva

---

## 📈 İlerleme Takibi

- **Haftalık Hedefler:**  
  Her aşama için 1-2 hafta ayırın, pratik projelerle ilerleyin.
- **Milestone Projeleri:**  
  Kişisel portföy, e-ticaret sayfası, blog şablonu, animasyonlu landing page.

---

## 🎯 Önemli İpuçları

- **Düzenli pratik yapın.**
- **Kod yazarak öğrenin.**
- **Projeler geliştirin.**
- **Topluluklara katılın ve soru sormaktan çekinmeyin.**
- **Farklı cihazlarda ve tarayıcılarda test yapın.**

---

## 🔗 Faydalı Linkler

- [MDN HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [MDN CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3Schools](https://www.w3schools.com/)
- [freeCodeCamp](https://www.freecodecamp.org/)
- [Frontend Mentor](https://www.frontendmentor.io/)
- [CSS Grid Generator](https://grid.layoutit.com/)
- [Flexbox Generator](https://flexbox.help/)

---

## 🎉 Sonuç

Bu rehberi takip ederek, HTML ve CSS konusunda sağlam bir temele sahip olabilir, modern ve profesyonel web arayüzleri geliştirebilirsiniz. **Unutmayın: En iyi öğrenme yolu, bol bol kod yazmak ve projeler üretmektir!**

**Başarılar! 🚀**

---
