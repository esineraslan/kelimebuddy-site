# KelimeBuddy — yasal sayfalar (geçici website)

Mağazaların istediği sayfalar: gizlilik politikası + KVKK aydınlatma metni, kullanım koşulları, web üzerinden hesap silme talimatı. Düz HTML/CSS; derleme adımı yok. Tam website MVP sonrası (`docs/10-roadmap.md` Faz 12).

| Dosya | Sayfa |
|---|---|
| `index.html` | Kısa tanıtım + bağlantılar |
| `gizlilik.html` | Gizlilik Politikası ve Aydınlatma Metni |
| `kosullar.html` | Kullanım Koşulları |
| `hesap-silme.html` | Hesap silme (Google Play "hesap silme URL'i") |

## Yayın

Ana repo gizli olduğu için sayfalar ayrı, herkese açık bir repodan GitHub Pages ile yayınlanır. Bu klasör tek kaynak; yayın reposuna `git subtree` ile gönderilir:

```bash
git subtree push --prefix kelimebuddy/apps/website site main
```

(`site` remote'u = herkese açık yayın reposu.)

## Metin sürümü

Sayfalardaki "Sürüm" tarihi, uygulamanın onay kaydında sakladığı sürümle aynı olmalıdır: `app_config.legal_versions` (`{"terms": "...", "privacy": "..."}`). Metin değiştiğinde ikisi birlikte güncellenir.

> Metinler hukuki görüş alınarak son hâline getirilmelidir (özellikle KVKK m.9 yurt dışı aktarım ve reşit olmayan kullanıcılar).
