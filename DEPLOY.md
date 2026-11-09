# Yayına alma

Bu klasör Hoop Zoo'nun gizlilik politikası ve destek sayfalarıdır. GitHub Pages'te
**oyunun adını taşıyan ayrı bir organizasyondan** yayınlanır; böylece adreste kişisel
isim geçmez (Happy BirThey'in `happybirthey.github.io` sitesi gibi, Goal Zoo da
`goal-zoo.github.io` kullanıyor).

## Adresler

| Sayfa | Adres |
| --- | --- |
| Privacy Policy (EN) | https://hoop-zoo.github.io/ |
| Gizlilik Politikası (TR) | https://hoop-zoo.github.io/gizlilik-politikasi/ |
| Help & Support (EN) | https://hoop-zoo.github.io/support/ |
| Yardım ve Destek (TR) | https://hoop-zoo.github.io/destek/ |

## Adımlar

1. GitHub'da (kendi hesabınla girişliyken) sağ üst **+ → New organization → Free**.
   Ad: **`hoop-zoo`**. Üyelikler varsayılan olarak gizlidir; öyle kalsın, böylece
   organizasyon sayfasında adın görünmez.
2. Organizasyonda **public** bir repo aç: **`hoop-zoo.github.io`** (ad birebir böyle
   olmalı). README, .gitignore ya da lisans ekleme; repo boş kalsın.
3. Bu klasörde:
   ```
   git remote add origin git@github.com:hoop-zoo/hoop-zoo.github.io.git
   git push -u origin main
   ```
4. Repo → **Settings → Pages**: Source "Deploy from a branch", `main` / `(root)`.
   `*.github.io` adlı repolarda bu genelde kendiliğinden açıktır.
5. 1–2 dakika sonra dört adresi de tarayıcıda aç.

Not: commit'lerin yazar adı repo geçmişinde görünür (`happybirthey.github.io`'da da
böyle). Adresin kendisinde isim yoktur.

## App Store Connect'e yazılacaklar

- **Privacy Policy URL**: İngilizce sayfa için `https://hoop-zoo.github.io/`, Türkçe
  sayfa için `https://hoop-zoo.github.io/gizlilik-politikasi/`
- **Support URL**: İngilizce `https://hoop-zoo.github.io/support/`, Türkçe
  `https://hoop-zoo.github.io/destek/`

Oyunun içindeki bağlantı (ebeveyn kapısının arkasında): `hoop-zoo/src/platform/links.ts`.

## Değiştirirken

- Politika değişirse iki dilde de **yürürlük tarihini** güncelle.
- İletişim adresi dört sayfada da geçiyor (`mailto:`); değişirse hepsinde değiştir.
- Sitede betik, web fontu, analitik ya da çerez olmasın: oyunun "hiçbir şey toplamayız"
  sözü siteyi de kapsar.
