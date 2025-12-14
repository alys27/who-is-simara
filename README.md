# Personal Portfolio Website (Jekyll)

SITE 1101 - İnformasiya Sistemləri Prinsipləri kursu üçün hazırlanmış şəxsi portfolyo veb-saytı.

**✨ Bu veb-sayt Jekyll ilə hazırlanmışdır (10% bonus üçün)**

## 📋 Təsvir

Bu veb-sayt Jekyll static site generator, HTML, CSS və JavaScript istifadə edərək hazırlanmışdır. Veb-sayt responsive dizayn ilə mobil, tablet və desktop cihazlarda yaxşı işləyir.

## 🚀 Xüsusiyyətlər

- ✅ Ana Səhifə (profil foto və mətn)
- ✅ Haqqımda səhifəsi (background, qualifications, activities)
- ✅ Layihələr səhifəsi (Project 1 və digər layihələr)
- ✅ Əlaqə səhifəsi
- ✅ Navigation bar və Footer
- ✅ GitHub və Codecademy icon linkləri
- ✅ Responsive dizayn (mobil və tablet üçün)
- ✅ Temiz və modulyar kod struktur
- ✅ **Jekyll static site generator** (10% bonus)

## 📁 Struktur

```
alys27.github.io/
├── _config.yml          # Jekyll konfiqurasiyası
├── _layouts/
│   └── default.html     # Əsas layout
├── _includes/
│   ├── header.html      # Navigation bar
│   └── footer.html      # Footer
├── index.html           # Ana səhifə
├── about.html           # Haqqımda səhifəsi
├── projects.html        # Layihələr səhifəsi
├── contact.html         # Əlaqə səhifəsi
├── css/
│   └── style.css        # Əsas CSS faylı
├── js/
│   └── main.js          # JavaScript faylı
├── images/              # Şəkillər qovluğu
│   ├── profile.jpg      # Profil şəkli
│   ├── project1.jpg     # Layihə 1 şəkli
│   ├── project2.jpg     # Layihə 2 şəkli
│   └── project3.jpg     # Layihə 3 şəkli
├── Gemfile              # Ruby dependencies
└── README.md            # Bu fayl
```

## 🔧 Quraşdırma

### Yerli İnkişaf Üçün

1. Ruby və Bundler quraşdırın:
   - Windows: [RubyInstaller](https://rubyinstaller.org/)
   - macOS: `brew install ruby`
   - Linux: `sudo apt-get install ruby-full`

2. Repository-ni klonlayın:
```bash
git clone https://github.com/alys27/alys27.github.io.git
cd alys27.github.io
```

3. Dependencies quraşdırın:
```bash
bundle install
```

4. Jekyll server-i başladın:
```bash
bundle exec jekyll serve
```

5. Brauzerdə açın: `http://localhost:4000`

### GitHub Pages-də Host Etmək

GitHub Pages avtomatik olaraq Jekyll build edir. Sadəcə:

1. Repository-ni GitHub-a push edin
2. Settings > Pages-də Jekyll seçin
3. Veb-saytınız hazır olacaq!

## 📝 Konfiqurasiya

Veb-saytı istifadə etmək üçün `_config.yml` faylında məlumatları dəyişdirməlisiniz:

```yaml
author: "Simara Aliyeva"
email: "your.email@example.com"
github_username: "alys27"
codecademy_username: "alyss27"
repository: "site1101-portfolio"
```

## 🌐 GitHub Pages

Veb-saytı GitHub Pages-də host etmək üçün:

1. GitHub repository-nizə gedin
2. Settings > Pages bölməsinə keçin
3. Source-dan "Deploy from a branch" seçin
4. Branch: `main` və folder: `/ (root)` seçin
5. Save düyməsini basın
6. GitHub Pages avtomatik olaraq Jekyll build edəcək
7. Bir neçə dəqiqə sonra veb-saytınız `https://alys27.github.io` ünvanında olacaq

## 📄 Lisenziya

Bu layihə təhsil məqsədi ilə hazırlanmışdır.

## 👤 Müəllif

[Adınız] - SITE 1101 Tələbəsi

## 🔗 Linklər

- [GitHub Profile](https://github.com/alys27)
- [Codecademy Profile](https://www.codecademy.com/profiles/alyss27)
- [Website Repository](https://github.com/alys27/alys27.github.io)

## 🎯 Jekyll Üstünlükləri

- ✅ Modulyar kod struktur (layouts və includes)
- ✅ Avtomatik site generation
- ✅ GitHub Pages-də native dəstək
- ✅ Markdown dəstəyi
- ✅ Liquid template engine
- ✅ Plugin sistemi
