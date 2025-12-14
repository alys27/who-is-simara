# Jekyll Quraşdırma Təlimatı

Bu veb-sayt Jekyll static site generator ilə hazırlanmışdır. Aşağıda quraşdırma və istifadə təlimatları verilmişdir.

## 🎯 Jekyll Nədir?

Jekyll Ruby əsaslı static site generator-dur. HTML, CSS və JavaScript-dən istifadə edərək statik veb-saytlar yaratmağa imkan verir. GitHub Pages-də native dəstəklənir.

## 📦 Quraşdırma

### Windows üçün:

1. **Ruby quraşdırın:**
   - [RubyInstaller](https://rubyinstaller.org/) yükləyin və quraşdırın
   - DevKit-i də quraşdırın

2. **Bundler quraşdırın:**
```bash
gem install bundler
```

3. **Dependencies quraşdırın:**
```bash
bundle install
```

### macOS üçün:

1. **Homebrew ilə Ruby quraşdırın:**
```bash
brew install ruby
```

2. **Bundler quraşdırın:**
```bash
gem install bundler
```

3. **Dependencies quraşdırın:**
```bash
bundle install
```

### Linux üçün:

1. **Ruby quraşdırın:**
```bash
sudo apt-get update
sudo apt-get install ruby-full build-essential zlib1g-dev
```

2. **Bundler quraşdırın:**
```bash
gem install bundler
```

3. **Dependencies quraşdırın:**
```bash
bundle install
```

## 🚀 İstifadə

### Yerli Server Başlatmaq

```bash
bundle exec jekyll serve
```

Veb-sayt `http://localhost:4000` ünvanında açılacaq.

### Build Etmək (Production)

```bash
bundle exec jekyll build
```

Build olunmuş fayllar `_site/` qovluğunda olacaq.

## 📝 Konfiqurasiya

`_config.yml` faylında aşağıdakı məlumatları dəyişdirin:

```yaml
title: Personal Portfolio
author: "[Adınız]"
email: "your.email@example.com"
github_username: "[YOUR_USERNAME]"
codecademy_username: "[YOUR_USERNAME]"
repository: "site1101-portfolio"
```

## 🏗️ Struktur

### Layouts (`_layouts/`)
- `default.html` - Əsas layout, bütün səhifələr üçün istifadə olunur

### Includes (`_includes/`)
- `header.html` - Navigation bar
- `footer.html` - Footer

### Pages
- `index.html` - Ana səhifə
- `about.html` - Haqqımda
- `projects.html` - Layihələr
- `contact.html` - Əlaqə

Hər səhifə front matter ilə başlayır:
```yaml
---
layout: default
title: Səhifə Adı
description: Səhifə təsviri
---
```

## 🔗 Linklər

Jekyll-də linklər `relative_url` filter ilə yaradılır:
```liquid
{{ '/about.html' | relative_url }}
```

Bu GitHub Pages-də subdirectory-də də düzgün işləyir.

## 🌐 GitHub Pages

GitHub Pages avtomatik olaraq Jekyll build edir:

1. Repository-ni GitHub-a push edin
2. Settings > Pages-də:
   - Source: "Deploy from a branch"
   - Branch: `main`
   - Folder: `/ (root)`
3. GitHub avtomatik olaraq Jekyll build edəcək

## 🐛 Problemlər və Həllər

### Problem: `bundle install` işləmir
**Həll:** Ruby və Bundler-in düzgün quraşdırıldığını yoxlayın:
```bash
ruby --version
bundle --version
```

### Problem: Jekyll server başlamır
**Həll:** Dependencies-in quraşdırıldığını yoxlayın:
```bash
bundle install
bundle exec jekyll serve
```

### Problem: Şəkillər görünmür
**Həll:** Şəkillərin yolunu `relative_url` filter ilə istifadə edin:
```liquid
{{ '/images/profile.jpg' | relative_url }}
```

### Problem: CSS/JS yüklənmir
**Həll:** Fayl yollarını `relative_url` filter ilə istifadə edin:
```liquid
{{ '/css/style.css' | relative_url }}
```

## 📚 Əlavə Resurslar

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Jekyll on GitHub Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
- [Liquid Template Language](https://shopify.github.io/liquid/)

## ✅ Yoxlama Siyahısı

- [ ] Ruby quraşdırılıb
- [ ] Bundler quraşdırılıb
- [ ] `bundle install` uğurla tamamlanıb
- [ ] `bundle exec jekyll serve` işləyir
- [ ] Veb-sayt `localhost:4000`-də açılır
- [ ] `_config.yml` düzgün konfiqurasiya edilib
- [ ] GitHub Pages-də Jekyll aktivdir

Uğurlar! 🎉

