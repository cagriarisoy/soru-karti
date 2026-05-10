# Soru Kartı Programı - GitHub Pages Sürümü

Bu sürüm, önceki tek dosyalık soru kartı uygulamasının GitHub Pages üzerinde yayınlanabilecek halidir.

## Özellikler

- Kullanıcı adı ve şifre ile giriş ekranı
- Her kullanıcı için ayrı kayıt alanı
- Kişiye özel JSON dışa aktarma: `soru_kartlari_kullaniciadi.json`
- JSON içe aktarma
- Mobil uyumlu arayüz
- iPhone Safari/Chrome için daha dayanıklı depolama kontrolü

## Varsayılan kullanıcılar

| Kullanıcı adı | Şifre |
|---|---|
| admin | 1234 |
| ogrenci1 | 1234 |
| ogrenci2 | 1234 |

Kullanıcıları değiştirmek için `users.json` dosyasını düzenleyin.

## GitHub Pages üzerinde yayınlama

1. GitHub'da yeni bir repository oluşturun.
2. Bu klasördeki `index.html`, `users.json`, `.nojekyll` ve `data` klasörünü repository içine yükleyin.
3. Repository sayfasında `Settings > Pages` bölümüne gidin.
4. Source olarak `Deploy from a branch` seçin.
5. Branch olarak `main`, folder olarak `/root` seçin ve kaydedin.
6. GitHub size bir yayın adresi verecektir.

## Önemli güvenlik notu

GitHub Pages statik site yayınlar. Bu nedenle bu sürüm gerçek anlamda güvenli çok kullanıcılı sistem değildir. `users.json` herkes tarafından görüntülenebilir. Şifreler açık metin olarak tutulmaz, hash olarak tutulur; ancak bu yine de gerçek güvenlik sağlamaz.

Gerçek kullanıcı hesabı, güvenli giriş ve sunucuda kullanıcıya özel dosya/kayıt için Firebase, Supabase, Appwrite, Vercel Functions veya kendi Node.js/PHP/Python sunucunuz gerekir.
