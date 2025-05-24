---

## Aşama 4: İleri Seviye CSS

**Süre:** 3-4 Hafta  
**Günlük Çalışma:** 1-2 saat

### 4.1 CSS Animations ve Transitions

#### CSS Transitions
```css
.button {
  background-color: blue;
  color: white;
  transition: all 0.3s ease;
}

.button:hover {
  background-color: red;
  transform: scale(1.05);
}

/* Spesifik özellikler için */
.element {
  transition-property: opacity, transform;
  transition-duration: 0.3s, 0.5s;
  transition-timing-function: ease-in-out;
  transition-delay: 0.1s;
}
```

#### CSS Animations
```css
/* Keyframes tanımlama */
@keyframes slideIn {
  0% {
    transform: translateX(-100%);
    opacity: 0;
  }
  100% {
    transform: translateX(0);
    opacity: 1;
  }
}

/* Animation uygulama */
.slide-element {
  animation: slideIn 0.5s ease-out forwards;
}

/* Kompleks animasyon */
.complex-animation {
  animation-name: slideIn;
  animation-duration: 2s;
  animation-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  animation-delay: 0.5s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}
```

#### Transform Özellikleri
```css
.transform-examples {
  /* 2D Transforms */
  transform: translate(50px, 100px);
  transform: rotate(45deg);
  transform: scale(1.5);
  transform: skew(10deg, 20deg);
  
  /* 3D Transforms */
  transform: rotateX(45deg);
  transform: rotateY(45deg);
  transform: translateZ(100px);
  
  /* Kombinasyon */
  transform: translate(50px, 50px) rotate(45deg) scale(1.2);
}
```

### 4.2 CSS Variables (Custom Properties)

#### Değişken Tanımlama ve Kullanma
```css
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --font-size-base: 16px;
  --spacing-unit: 8px;
  --border-radius: 4px;
}

.component {
  color: var(--primary-color);
  font-size: var(--font-size-base);
  padding: calc(var(--spacing-unit) * 2);
  border-radius: var(--border-radius);
}

/* Fallback değerler */
.element {
  color: var(--undefined-color, #000000);
}
```

#### Dinamik Değişkenler
```css
/* JavaScript ile değiştirilebilir */
.theme-dark {
  --bg-color: #2c3e50;
  --text-color: #ecf0f1;
}

.theme-light {
  --bg-color: #ffffff;
  --text-color: #2c3e50;
}
```

### 4.3 CSS Preprocessors (Sass/SCSS)

#### Variables
```scss
// Değişkenler
$primary-color: #3498db;
$font-stack: 'Helvetica Neue', sans-serif;
$base-font-size: 16px;

body {
  font: $base-font-size $font-stack;
  color: $primary-color;
}
```

#### Nesting
```scss
.navbar {
  background-color: $primary-color;
  
  ul {
    list-style: none;
    
    li {
      display: inline-block;
      
      a {
        text-decoration: none;
        
        &:hover {
          color: white;
        }
      }
    }
  }
}
```

#### Mixins
```scss
@mixin button-style($bg-color, $text-color) {
  background-color: $bg-color;
  color: $text-color;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  
  &:hover {
    opacity: 0.8;
  }
}

.primary-button {
  @include button-style(#3498db, white);
}
```

### 4.4 CSS Metodolojileri

#### BEM (Block Element Modifier)
```html
<!-- HTML -->
<div class="card">
  <h2 class="card__title">Başlık</h2>
  <p class="card__content">İçerik</p>
  <button class="card__button card__button--primary">Buton</button>
</div>
```

```scss
// SCSS
.card {
  border: 1px solid #ddd;
  border-radius: 4px;
  # HTML ve CSS Öğrenme Yol Haritası

## İçindekiler

1. [Genel Bakış](#genel-bakış)
2. [Temel Kaynaklar](#temel-kaynaklar)
3. [Aşama 1: HTML Temelleri](#aşama-1-html-temelleri)
4. [Aşama 2: CSS Temelleri](#aşama-2-css-temelleri)
5. [Aşama 3: Responsive Tasarım](#aşama-3-responsive-tasarım)
6. [Aşama 4: İleri Seviye CSS](#aşama-4-ileri-seviye-css)
7. [Pratik Araçlar](#pratik-araçlar)
8. [İlerleme Takibi](#ilerleme-takibi)
9. [Önemli İpuçları](#önemli-ipuçları)
10. [Faydalı Linkler](#faydalı-linkler)
11. [Sonuç](#sonuç)

---

## Genel Bakış

Bu yol haritası, HTML ve CSS'i sıfırdan öğrenip profesyonel seviyeye ulaşmak için tasarlanmıştır. Yaklaşık **3-6 ay** içinde tamamlanabilir.

### Hedef Kitle

- Web geliştirmeye yeni başlayanlar
- HTML ve CSS temellerini öğrenmek isteyenler
- Frontend geliştirme yolculuğuna başlayanlar

### Gereksinimler

- Temel bilgisayar kullanım becerisi
- İnternet bağlantısı
- Günlük 1-2 saat zaman ayırabilmek

---

## Temel Kaynaklar

### Türkçe Kaynaklar

#### YouTube Kanalları

- **Engin Demirok** - HTML/CSS Eğitim Serisi
- **Yazılım Bilimi** - Web Geliştirme
- **Geleceği Yazanlar** - Frontend Eğitimleri
- **Kablosuz Kedi** - Web Tasarım

#### Türkçe Web Siteleri

- **Kodluyoruz** - Ücretsiz eğitim platformu
- **BTK Akademi** - Devlet destekli ücretsiz kurslar

### İngilizce Kaynaklar

#### Dokümantasyon

- **MDN Web Docs** (`developer.mozilla.org`) - En kapsamlı dokümantasyon
- **W3Schools** (`w3schools.com`) - Başlangıç dostu
- **CSS-Tricks** (`css-tricks.com`) - CSS ipuçları ve rehberler

#### Online Kurslar

- **freeCodeCamp** - Ücretsiz interaktif kurslar
- **Codecademy** - Interaktif öğrenme
- **Khan Academy** - Temel web geliştirme

### Kitaplar

#### Türkçe

- "HTML5 ve CSS3 ile Web Tasarımı" - Kodlab Yayınları
- "Web Tasarım ve Programlama" - Seçkin Yayıncılık

#### İngilizce

- "CSS: The Definitive Guide" - Eric Meyer
- "HTML and CSS: Design and Build Websites" - Jon Duckett

---

## Aşama 1: HTML Temelleri

**Süre:** 2-3 Hafta  
**Günlük Çalışma:** 1-2 saat

### 1.1 HTML'e Giriş

#### Öğrenilecek Konular

- HTML nedir ve nasıl çalışır?
- Web tarayıcıları ve HTML ilişkisi
- Temel HTML belge yapısı
- HTML dosyası oluşturma ve kaydetme

#### Pratik Alıştırmalar

- İlk HTML dosyanızı oluşturun
- Tarayıcıda açıp test edin
- HTML yapısını kavrayın

### 1.2 Temel HTML Etiketleri

#### Zorunlu Etiketler

```html
<html>, <head>, <body>
<title>, <meta>
```

#### İçerik Etiketleri

```html
<h1>
  -
  <h6>
    <!-- Başlık etiketleri -->
    <p>
      <!-- Paragraf -->
      <a>
        <!-- Bağlantılar -->
        <img />
        <!-- Görsel -->
        <ul>
          ,
          <ol>
            ,
            <li><!-- Listeler --></li>
          </ol>
        </ul></a
      >
    </p>
  </h6>
</h1>
```

### 1.3 Metin Biçimlendirme

#### Biçimlendirme Etiketleri

```html
<strong>
  <!-- Kalın metin -->
  <em>
    <!-- Vurgulu metin -->
    <mark>
      <!-- İşaretli metin -->
      <span>
        <!-- Satır içi bölüm -->
        <div>
          <!-- Blok bölüm -->
          <br />
          <!-- Satır kesme -->
          <hr />
          <!-- Yatay çizgi -->
        </div></span
      ></mark
    ></em
  ></strong
>
```

### 1.4 HTML Formları

#### Form Bileşenleri

```html
<form>      <!-- Form kapsayıcısı -->
<input>     <!-- Giriş alanları -->
<textarea>  <!-- Çok satırlı metin -->
<select>, <option>  <!-- Açılır menü -->
<button>    <!-- Düğme -->
```

#### Form Doğrulama

- `required` özelliği
- Input türleri (`email`, `tel`, `url`)
- Pattern validation

### 1.5 Semantic HTML

#### Yapısal Etiketler

```html
<header>
  <!-- Sayfa başlığı -->
  <nav>
    <!-- Navigasyon -->
    <main>
      <!-- Ana içerik -->
      <section>
        <!-- Bölüm -->
        <article>
          <!-- Makale -->
          <aside>
            <!-- Yan panel -->
            <footer><!-- Sayfa alt bilgisi --></footer>
          </aside>
        </article>
      </section>
    </main>
  </nav>
</header>
```

### 1.6 Pratik Projeler

#### Proje 1: Kişisel CV Sayfası

- **Hedef:** HTML etiketlerini kullanarak CV oluşturmak
- **İçerik:** Kişisel bilgiler, eğitim, deneyim, yetenekler
- **Kullanılacak Etiketler:** `h1-h6`, `p`, `ul`, `ol`, `strong`, `em`

#### Proje 2: Basit Blog Yazısı

- **Hedef:** Semantic HTML kullanarak blog yazısı yazmak
- **İçerik:** Başlık, yazı içeriği, görsel, yazar bilgisi
- **Kullanılacak Etiketler:** `article`, `header`, `main`, `img`, `p`

#### Proje 3: İletişim Formu

- **Hedef:** Çalışan bir iletişim formu oluşturmak
- **İçerik:** Ad, email, mesaj alanları, gönder butonu
- **Kullanılacak Etiketler:** `form`, `input`, `textarea`, `button`

### 1.7 Değerlendirme Kriterleri

#### Bu aşamayı tamamladıysanız

- [ ] HTML dosyası oluşturup tarayıcıda açabiliyorsunuz
- [ ] Temel HTML etiketlerini kullanabiliyorsunuz
- [ ] Semantic HTML yapısını anlıyorsunuz
- [ ] Basit formlar oluşturabiliyorsunuz
- [ ] HTML kodlarınız hatasız çalışıyor

---

## Aşama 2: CSS Temelleri

**Süre:** 3-4 Hafta  
**Günlük Çalışma:** 1-2 saat

### 2.1 CSS'e Giriş

#### CSS Nedir?

- Cascading Style Sheets
- HTML ile görsel tasarım ayrımı
- CSS'in avantajları ve kullanım alanları

#### CSS Ekleme Yöntemleri

```html
<!-- Inline CSS -->
<p style="color: red;">Kırmızı metin</p>

<!-- Internal CSS -->
<style>
  p {
    color: red;
  }
</style>

<!-- External CSS (Önerilen) -->
<link rel="stylesheet" href="style.css" />
```

### 2.2 CSS Seçiciler (Selectors)

#### Temel Seçiciler

```css
/* Element seçici */
p {
  color: blue;
}

/* Class seçici */
.highlight {
  background-color: yellow;
}

/* ID seçici */
#header {
  font-size: 24px;
}

/* Universal seçici */
* {
  margin: 0;
  padding: 0;
}
```

#### Kombinasyon Seçiciler

```css
/* Descendant */
div p {
  color: red;
}

/* Child */
div > p {
  color: blue;
}

/* Adjacent sibling */
h1 + p {
  margin-top: 0;
}
```

### 2.3 Temel CSS Özellikleri

#### Renkler

```css
.element {
  color: red; /* Metin rengi */
  background-color: #ff0000; /* Arka plan rengi */
  background-color: rgb(255, 0, 0);
  background-color: rgba(255, 0, 0, 0.5);
}
```

#### Yazı Tipleri

```css
.text {
  font-family: Arial, sans-serif;
  font-size: 16px;
  font-weight: bold;
  font-style: italic;
  text-align: center;
  line-height: 1.5;
}
```

#### Kenarlıklar

```css
.border-example {
  border: 2px solid black;
  border-radius: 5px;
  border-top: 1px dashed red;
}
```

### 2.4 CSS Box Model

#### Box Model Bileşenleri

```css
.box {
  width: 200px; /* İçerik genişliği */
  height: 100px; /* İçerik yüksekliği */
  padding: 20px; /* İç boşluk */
  border: 2px solid black; /* Kenarlık */
  margin: 10px; /* Dış boşluk */
}
```

#### Box Sizing

```css
* {
  box-sizing: border-box; /* Önerilen yaklaşım */
}
```

### 2.5 Pozisyonlama

#### Position Değerleri

```css
.static {
  position: static;
} /* Varsayılan */
.relative {
  position: relative;
} /* Göreceli */
.absolute {
  position: absolute;
} /* Mutlak */
.fixed {
  position: fixed;
} /* Sabit */
.sticky {
  position: sticky;
} /* Yapışkan */
```

#### Z-Index

```css
.layer1 {
  z-index: 1;
}
.layer2 {
  z-index: 2;
}
```

### 2.6 Pseudo-Classes ve Pseudo-Elements

#### Pseudo-Classes

```css
a:hover {
  color: red;
}
input:focus {
  border-color: blue;
}
li:first-child {
  font-weight: bold;
}
tr:nth-child(even) {
  background-color: #f2f2f2;
}
```

#### Pseudo-Elements

```css
p::first-line {
  font-weight: bold;
}
p::before {
  content: "★ ";
}
p::after {
  content: " ★";
}
```

### 2.7 Pratik Projeler

#### Proje 1: HTML Sayfalarını Güzelleştirme

- **Hedef:** Önceki HTML projelerine CSS eklemek
- **Görevler:**
  - Renk şeması oluşturma
  - Yazı tiplerini düzenleme
  - Boşlukları ayarlama
  - Kenarlık ve gölge efektleri

#### Proje 2: Basit Kart Tasarımları

- **Hedef:** Modern kart bileşenleri oluşturmak
- **İçerik:** Ürün kartları, profil kartları, blog kartları
- **Teknikler:** Box model, shadow, border-radius

#### Proje 3: Navigation Bar

- **Hedef:** Responsive navigasyon menüsü
- **Özellikler:** Hover efektleri, active states
- **Teknikler:** Flexbox temellerı, pseudo-classes

### 2.8 Değerlendirme Kriterleri

#### Bu aşamayı tamamladıysanız

- [ ] CSS dosyası oluşturup HTML'e bağlayabiliyorsunuz
- [ ] Temel CSS özelliklerini kullanabiliyorsunuz
- [ ] Box model'i anlıyor ve uygulayabiliyorsunuz
- [ ] Farklı seçici türlerini kullanabiliyorsunuz
- [ ] Basit hover efektleri oluşturabiliyorsunuz

---

## Aşama 3: Responsive Tasarım

**Süre:** 2-3 Hafta  
**Günlük Çalışma:** 1-2 saat

### 3.1 Flexbox Layout

#### Flexbox Temelleri

```css
.container {
  display: flex;
  flex-direction: row; /* row, column, row-reverse, column-reverse */
  justify-content: center; /* flex-start, flex-end, center, space-between, space-around */
  align-items: center; /* flex-start, flex-end, center, stretch, baseline */
  flex-wrap: wrap; /* nowrap, wrap, wrap-reverse */
}
```

#### Flex Items

```css
.flex-item {
  flex-grow: 1; /* Büyüme oranı */
  flex-shrink: 0; /* Küçülme oranı */
  flex-basis: 200px; /* Temel boyut */

  /* Kısayol */
  flex: 1 0 200px; /* grow shrink basis */
}
```

### 3.2 CSS Grid Layout

#### Grid Container

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr; /* Sütun boyutları */
  grid-template-rows: auto 1fr auto; /* Satır boyutları */
  gap: 20px; /* Boşluk */
  grid-template-areas:
    "header header header"
    "sidebar content content"
    "footer footer footer";
}
```

#### Grid Items

```css
.grid-item {
  grid-column: 1 / 3; /* Sütun span */
  grid-row: 1 / 2; /* Satır span */
  grid-area: header; /* Alan adı */
}
```

### 3.3 Media Queries

#### Temel Syntax

```css
/* Mobile First Yaklaşım */
.container {
  width: 100%;
  padding: 10px;
}

/* Tablet */
@media screen and (min-width: 768px) {
  .container {
    width: 750px;
    margin: 0 auto;
  }
}

/* Desktop */
@media screen and (min-width: 1024px) {
  .container {
    width: 1000px;
  }
}
```

#### Yaygın Breakpoint'ler

```css
/* Ekstra küçük cihazlar (telefonlar) */
@media (max-width: 575.98px) {
}

/* Küçük cihazlar (landscape telefonlar) */
@media (min-width: 576px) and (max-width: 767.98px) {
}

/* Orta cihazlar (tabletler) */
@media (min-width: 768px) and (max-width: 991.98px) {
}

/* Büyük cihazlar (masaüstü) */
@media (min-width: 992px) and (max-width: 1199.98px) {
}

/* Ekstra büyük cihazlar (büyük masaüstü) */
@media (min-width: 1200px) {
}
```

### 3.4 Modern CSS Units

#### Viewport Units

```css
.element {
  width: 50vw; /* Viewport width'in %50'si */
  height: 100vh; /* Viewport height'in %100'ü */
  font-size: 4vmin; /* vw ve vh'nin küçüğünün %4'ü */
  margin: 2vmax; /* vw ve vh'nin büyüğünün %2'si */
}
```

#### Relative Units

```css
.element {
  font-size: 1.2em; /* Parent element'in 1.2 katı */
  padding: 2rem; /* Root element'in 2 katı */
  width: 75%; /* Parent'in %75'i */
}
```

#### Grid fr Unit

```css
.grid {
  grid-template-columns: 1fr 2fr 1fr; /* Esnek oranlar */
}
```

### 3.5 Responsive Images

#### Flexible Images

```css
img {
  max-width: 100%;
  height: auto;
}
```

#### Picture Element

```html
<picture>
  <source media="(min-width: 768px)" srcset="large.jpg" />
  <source media="(min-width: 480px)" srcset="medium.jpg" />
  <img src="small.jpg" alt="Responsive image" />
</picture>
```

### 3.6 Pratik Projeler

#### Proje 1: Responsive Kart Galeri

- **Hedef:** Farklı ekran boyutlarında düzgün görünen kart sistemi
- **Teknikler:** CSS Grid, Media Queries
- **Özellikler:**
  - Mobile: 1 sütun
  - Tablet: 2 sütun
  - Desktop: 3-4 sütun

#### Proje 2: Mobile-Friendly Navigation

- **Hedef:** Hamburger menü ile responsive navigation
- **Teknikler:** Flexbox, Media Queries, CSS Transforms
- **Özellikler:**
  - Mobile: Hamburger menü
  - Desktop: Yatay menü

#### Proje 3: Responsive Blog Layout

- **Hedef:** Modern blog tasarımı
- **Teknikler:** CSS Grid, Flexbox kombinasyonu
- **Bölümler:** Header, sidebar, main content, footer

### 3.7 Değerlendirme Kriterleri

#### Bu aşamayı tamamladıysanız

- [ ] Flexbox ile layout oluşturabiliyorsunuz
- [ ] CSS Grid temellerini kullanabiliyorsunuz
- [ ] Media queries yazabiliyorsunuz
- [ ] Mobile-first yaklaşımını anlıyorsunuz
- [ ] Responsive images kullanabiliyorsunuz

---

## 🚀 Aşama 4: İleri Seviye CSS (3-4 Hafta)

### Öğrenilecek Konular:

1. **CSS Animations ve Transitions**

   - `transition` özellikleri
   - `@keyframes` ve `animation`
   - Transform özellikleri
   - Easing functions

2. **CSS Preprocessors**

   - Sass/SCSS temelleri
   - Variables, nesting, mixins
   - Partials ve imports

3. **CSS Metodolojileri**

   - BEM (Block Element Modifier)
   - CSS organizasyonu
   - Naming conventions

4. **Modern CSS Features**
   - CSS Variables (Custom Properties)
   - CSS Grid advanced
   - CSS Subgrid
   - Container Queries

### Pratik Projeler:

- Animasyonlu landing page
- Interactive hover effects
- Complex grid layouts

---

## 🛠️ Pratik Araçlar

### Code Editors:

- **VS Code** (önerilen) - Ücretsiz, güçlü
- **Sublime Text**
- **Atom**

### VS Code Eklentileri:

- Live Server
- HTML CSS Support
- Auto Rename Tag
- Prettier
- Emmet

### Online Editörler:

- **CodePen** - CSS denemeleri için
- **JSFiddle**
- **Repl.it**

### Design Araçları:

- **Figma** - UI tasarım
- **Adobe XD**
- **Canva** - Basit tasarımlar

---

## 📈 İlerleme Takibi

### Haftalık Hedefler:

- **1-2. Hafta:** HTML temelleri, basit sayfalar
- **3-4. Hafta:** CSS temelleri, styling
- **5-6. Hafta:** Layout ve positioning
- **7-8. Hafta:** Responsive design
- **9-10. Hafta:** Animasyonlar ve ileri CSS
- **11-12. Hafta:** Proje geliştirme

### Milestone Projeleri:

1. **Kişisel Portföy Sitesi** (HTML + CSS)
2. **Responsive E-ticaret Ürün Sayfası**
3. **Modern Blog Template**
4. **Landing Page with Animations**

---

## 🎯 Önemli İpuçları

### Öğrenme Stratejileri:

- **Günlük 1-2 saat** düzenli çalışma
- **Kod yazarak öğrenme** - sadece okumak yetmez
- **Projeler üzerinden pratik yapma**
- **Developer tools** kullanmayı öğrenme
- **Community'lere katılma** (Stack Overflow, Reddit)

### Sık Yapılan Hatalar:

- Çok fazla teori, az praktik
- Responsive tasarımı ihmal etme
- Semantic HTML kullanmama
- CSS organizasyonuna dikkat etmeme
- Cross-browser uyumluluğu test etmeme

### Motivasyon için:

- Küçük hedefler koyma
- İlerlemeyi görselleştirme
- Başkalarının kodlarını inceleme
- Online topluluklara katılma
- Kendi projelerinizi paylaşma

---

## 🔗 Faydalı Linkler

### Dokumentasyon:

- [MDN HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [MDN CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3Schools](https://www.w3schools.com/)

### Practice Siteleri:

- [freeCodeCamp](https://www.freecodecamp.org/)
- [Codecademy](https://www.codecademy.com/)
- [Frontend Mentor](https://www.frontendmentor.io/)

### Design İnspirasyonu:

- [Dribbble](https://dribbble.com/)
- [Behance](https://www.behance.net/)
- [Awwwards](https://www.awwwards.com/)

### CSS Generators:

- [CSS Grid Generator](https://grid.layoutit.com/)
- [Flexbox Generator](https://flexbox.help/)
- [Box Shadow Generator](https://box-shadow.dev/)

---

## 🎉 Sonuç

Bu yol haritasını takip ederek 3-6 ay içinde HTML ve CSS konularında yetkin hale gelebilirsiniz. Unutmayın ki en önemli şey **düzenli pratik yapmak** ve **projeler geliştirmek**tir. Kod yazmaya başlayın ve öğrendiklerinizi hemen uygulayın!

**Başarılar! 🚀**
