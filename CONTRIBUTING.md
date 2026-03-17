# Katkıda Bulunma Rehberi

Bu doküman, **TFN-Software-Team** organizasyonundaki tüm repolar için geçerli olan geliştirme kurallarını ve iş akışını açıklar.

---

## Branch İsimlendirme Kuralları

Yeni bir branch oluştururken aşağıdaki formatı kullanın:

| Tür | Format | Örnek |
|-----|--------|-------|
| Yeni özellik | `feature/<kisa-aciklama>` | `feature/motor-kontrol` |
| Hata düzeltme | `bugfix/<kisa-aciklama>` | `bugfix/sensor-okuma-hatasi` |
| Acil düzeltme | `hotfix/<kisa-aciklama>` | `hotfix/kritik-baglanti-sorunu` |
| Dokümantasyon | `docs/<kisa-aciklama>` | `docs/kurulum-rehberi` |
| Refaktör | `refactor/<kisa-aciklama>` | `refactor/veri-katmani` |

> **Not:** Branch isimleri küçük harfle, Türkçe karakter kullanmadan ve boşluk yerine `-` ile yazılır.

---

## Commit Mesajı Formatı

Commit mesajlarınızda şu formata uymanız önerilir:

```
<tip>: <kısa açıklama>
```

**Tip seçenekleri:**

| Tip | Açıklama |
|-----|----------|
| `feat` | Yeni özellik |
| `fix` | Hata düzeltme |
| `docs` | Dokümantasyon değişikliği |
| `refactor` | Kod iyileştirme (fonksiyonda değişiklik yok) |
| `test` | Test ekleme veya düzeltme |
| `chore` | Yapılandırma, bağımlılık vb. |

**Örnekler:**
```
feat: CAN bus haberleşme modülü eklendi
fix: sıcaklık sensörü okuması düzeltildi
docs: kurulum adımları güncellendi
```

---

## Pull Request (PR) İş Akışı

1. `main` branch'inden yeni bir branch oluşturun (yukarıdaki kurallara uygun).
2. Değişikliklerinizi yapın ve commit'leyin.
3. Branch'inizi push edin ve **Pull Request** açın.
4. PR şablonunu eksiksiz doldurun.
5. En az **1 kişinin onayı (review)** alındıktan sonra `main`'e merge edilir.

> ⚠️ `main` branch'ine doğrudan push yapılması yasaktır. Tüm değişiklikler PR üzerinden geçmelidir.

---

## Kod İnceleme (Code Review) Kuralları

- Her PR en az **1 onay** almalıdır.
- Reviewer, kodun çalışıp çalışmadığını değil, **okunabilirliğini** ve **mimariye uygunluğunu** da kontrol etmelidir.
- Geri bildirimlerde yapıcı ve açıklayıcı olun.
- Eğer kritik bir değişiklik varsa ilgili takım liderine mention atın.

---

## Genel Kurallar

- **Türkçe karakter** dosya ve branch adlarında kullanılmaz (ç, ş, ğ, ı, ö, ü yerine c, s, g, i, o, u).
- Projeye özgü kurallar varsa ilgili repo'nun kendi `README.md` dosyasında belirtilir.
- Sorularınız için Prytaneion reposunda bir **Issue** açabilirsiniz.
