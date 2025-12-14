# Veb-sayt Quraşdırma Təlimatı (Jekyll)

Bu təlimat Jekyll ilə hazırlanmış veb-saytı fərdiləşdirmək və GitHub Pages-də host etmək üçün addım-addım təlimatlar verir.

**✨ Bu veb-sayt Jekyll ilə hazırlanmışdır (10% bonus üçün)**

## 📝 Addım 1: Şəxsi Məlumatları Dəyişdirmək

### 1.1 `_config.yml` Faylını Konfiqurasiya Etmək

Jekyll-də bütün konfiqurasiya `_config.yml` faylındadır. Bu faylı açın və aşağıdakı məlumatları dəyişdirin:

```yaml
title: Personal Portfolio
author: "Simara Aliyeva"
email: "saliyeva24095@ada.edu.az"
github_username: "alys27"
codecademy_username: "alyss27"
repository: "alys27.github.io"
```

**Qeyd:** Jekyll-də məlumatlar `_config.yml`-dən avtomatik olaraq bütün səhifələrə tətbiq olunur. Ayrı-ayrı HTML fayllarında dəyişiklik etməyə ehtiyac yoxdur!

### 1.2 HTML Səhifələrində Məzmunu Dəyişdirmək

HTML səhifələrində (`about.html`, `projects.html` və s.) məzmunu fərdiləşdirin:

- `about.html` - Universitet adı, təhsil tarixləri, fəaliyyətlər
- `projects.html` - Layihə adları, təsvirlər, texnologiyalar
- `contact.html` - Əlavə əlaqə məlumatları (əgər lazımdırsa)

**Qeyd:** `_config.yml`-dəki məlumatlar avtomatik olaraq bütün səhifələrdə istifadə olunur (`{{ site.github_username }}` və s.)

## 📸 Addım 2: Şəkilləri Əlavə Etmək

1. `images/` qovluğuna öz şəkillərinizi əlavə edin:
   - `profile.jpg` - Profil şəkliniz (250x250px və ya kvadrat)
   - `project1.jpg` - Layihə 1 şəkli
   - `project2.jpg` - Layihə 2 şəkli (opsional)
   - `project3.jpg` - Digər layihə şəkli (opsional)

2. Şəkillərin adlarının dəqiq olmasına diqqət edin (böyük/kiçik hərf)

## 🔧 Addım 3: Jekyll Quraşdırması (Yerli İnkişaf üçün)

### 3.1 Ruby və Bundler Quraşdırmaq

**Windows:**
- [RubyInstaller](https://rubyinstaller.org/) yükləyin və quraşdırın

**macOS:**
```bash
brew install ruby
```

**Linux:**
```bash
sudo apt-get install ruby-full
```

### 3.2 Dependencies Quraşdırmaq

```bash
gem install bundler
bundle install
```

### 3.3 Yerli Server Başlatmaq

```bash
bundle exec jekyll serve
```

Veb-sayt `http://localhost:4000` ünvanında açılacaq.

## 🔧 Addım 4: Git Repository Yaratmaq

### 3.1 Git İlkin Quraşdırması

```bash
# Git konfiqurasiyası (ilk dəfə istifadə edirsinizsə)
git config --global user.name "Adınız"
git config --global user.email "email@example.com"
```

### 3.2 Repository Yaratmaq

```bash
# Qovluğa daxil olun
cd "C:\Users\Administrator\Desktop\projeckt simare"

# Git repository başlatın
git init

# Bütün faylları əlavə edin
git add .

# İlk commit edin
git commit -m "Initial commit: Personal portfolio website"

# GitHub-da yeni repository yaradın (github.com-da)
# Sonra remote əlavə edin
git remote add origin https://github.com/alys27/alys27.github.io.git

# Branch adını main olaraq dəyişdirin
git branch -M main

# GitHub-a göndərin
git push -u origin main
```

## 🌐 Addım 5: GitHub Pages Aktivləşdirmək

1. GitHub repository-nizə gedin
2. **Settings** (Parametrlər) düyməsinə basın
3. Sol menyudan **Pages** seçin
4. **Source** bölməsində:
   - **Deploy from a branch** seçin
   - Branch: `main` seçin
   - Folder: `/ (root)` seçin
5. **Save** düyməsinə basın
6. GitHub avtomatik olaraq Jekyll build edəcək
7. Bir neçə dəqiqə gözləyin (build prosesi 1-2 dəqiqə çəkə bilər)
8. Veb-saytınız `https://alys27.github.io` ünvanında olacaq

**Qeyd:** 
- GitHub Pages avtomatik olaraq Jekyll build edir
- Əgər artıq `[YOUR_USERNAME].github.io` ünvanında veb-saytınız varsa, bu layihəni subdirectory-də host edin
- Build prosesini Actions tab-ında izləyə bilərsiniz

## 💾 Addım 6: Commit-lər Yaratmaq

Layihə inkişafı zamanı commit-lər yaratmağı unutmayın:

```bash
# Dəyişiklikləri yoxlayın
git status

# Dəyişiklikləri əlavə edin
git add .

# Commit edin
git commit -m "Açıqlayıcı mesaj (məsələn: About səhifəsini tamamladım)"

# GitHub-a göndərin
git push
```

**Məsləhət:** Hər mühüm dəyişiklikdən sonra commit edin:
- Yeni səhifə əlavə etdikdə
- Dizayn dəyişiklikləri etdikdə
- Şəkillər əlavə etdikdə
- Məzmun yeniləmələri etdikdə

## 📤 Addım 7: AI Chat Export

1. Cursor-də (və ya VSCode-da) AI chat pəncərəsini açın
2. Export/Chat Export seçimini tapın
3. Chat-i markdown (.md) formatında export edin
4. Export olunmuş faylı layihə qovluğuna saxlayın (məsələn: `ai-chat-export.md`)

## ✅ Addım 8: Yoxlama Siyahısı

Təqdim etməzdən əvvəl yoxlayın:

- [ ] `_config.yml` faylında bütün məlumatlar doldurulub
- [ ] GitHub username, Codecademy username düzgündür
- [ ] Profil şəkli əlavə edilib
- [ ] Layihə şəkilləri əlavə edilib
- [ ] GitHub repository public-dir
- [ ] GitHub Pages aktivdir və işləyir
- [ ] Bütün linklər düzgün işləyir
- [ ] Responsive dizayn mobil cihazlarda yoxlanılıb
- [ ] AI chat export faylı hazırdır
- [ ] Bir neçə commit GitHub-da görünür

## 🔗 Təqdim Linkləri

Təqdim edərkən aşağıdakı linkləri hazırlayın:

1. **Veb-sayt linki:**
   ```
   https://alys27.github.io
   ```

2. **GitHub repository linki:**
   ```
   https://github.com/alys27/alys27.github.io
   ```

3. **AI chat export faylı:**
   - Fayl adı: `ai-chat-export.md` (və ya oxşar)

## 🆘 Problemlər və Həllər

### Problem: Şəkillər görünmür
**Həll:** Şəkillərin fayl adlarının və yolunun düzgün olduğunu yoxlayın. Fayl adları böyük/kiçik hərfə həssasdır.

### Problem: GitHub Pages işləmir
**Həll:** 
- Repository-nin public olduğunu yoxlayın
- Settings > Pages-də "Deploy from a branch" seçildiyini yoxlayın
- Branch və folder düzgün seçildiyini yoxlayın
- Actions tab-ında build prosesini yoxlayın (əgər error varsa görünəcək)
- Bir neçə dəqiqə gözləyin (Jekyll build prosesi zaman ala bilər)

### Problem: Navigation menu mobil cihazlarda işləmir
**Həll:** JavaScript faylının (`js/main.js`) düzgün yükləndiyini yoxlayın.

### Problem: Stil tətbiq olunmur
**Həll:** CSS faylının (`css/style.css`) yolunun düzgün olduğunu yoxlayın.

## 📚 Əlavə Resurslar

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Jekyll on GitHub Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
- [Git Tutorial](https://www.youtube.com/watch?v=8JJ101D3knE)
- [HTML/CSS Tutorial](https://www.youtube.com/watch?v=PlxWf493en4)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Personal Site Examples](https://personalsit.es/)

Uğurlar! 🎉

