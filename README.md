# Prytaneion

> *Antik Yunan şehir-devletlerinde **Prytaneion**, kentin kutsal ateşinin yandığı ve tüm yönetim kararlarının alındığı merkez yapıydı.*

**TFN-Software-Team** organizasyonunun yönetim merkezi. Tıpkı adını aldığı yapı gibi, organizasyonun tüm otomasyon süreçleri ve iş akışları bu repodan yönetilir.

---

## Prytaneion Nedir?

**Prytaneion**, TUFAN Elektromobil ve LİKYA Otonom Araç takımlarının GitHub organizasyonu olan [TFN-Software-Team](https://github.com/TFN-Software-Team) için oluşturulmuş yönetim merkezidir. Bu repo üzerinden:

- 🆕 Yeni repo talepleri oluşturulur ve otomatik onaylanır
- 🐛 Hata raporları ve özellik talepleri standart şablonlarla açılır
- 📋 Organizasyon genelindeki iş akışları ve kurallar dokümante edilir

---

## Mevcut İş Akışları

### 🆕 Yeni Repository Açma Talebi
Organizasyon içinde yeni bir repo oluşturmak için:

1. Bu reponun **Issues** sekmesine gidin → **New Issue**.
2. **"Yeni Repo Talebi (Public)"** şablonunu seçin.
3. Şablon içindeki YAML bloğunu doldurun:
   ```yaml
   TAKIM: <TUFAN-veya-LIKYA>
   PROJE: <Repo-adi>
   MAINTAINER: <github-kullanici-adi>
   ```
4. Talebi oluşturun (Submit).
5. Bir organizasyon yöneticisi (Owner) issue'ya `/repo-onay` yorumunu atacaktır.
6. GitHub Action otomatik olarak `<TAKIM>-<PROJE>` adıyla yeni bir public repo oluşturur, belirtilen kişiyi **Maintainer** olarak ekler ve `main` branch'ine koruma kurallarını uygular.

---

## Issue Şablonları

| Şablon | Açıklama |
|--------|----------|
| **Yeni Repo Talebi** | TUFAN veya LİKYA için yeni repository oluşturma |
| **Hata Raporu (Bug Report)** | Bir hata veya beklenmeyen davranış bildirme |
| **Özellik / İyileştirme Talebi** | Yeni özellik veya iyileştirme önerisi |

---

## PR (Pull Request) Şablonu

Tüm PR'larda otomatik olarak yüklenen standart bir kontrol listesi mevcuttur. PR açarken:
- Değişiklik özetini yazın
- Değişiklik türünü işaretleyin (Bug Fix, Feature, Docs, vb.)
- Kontrol listesini tamamlayın
- İlgili issue'yu linkleyin

---

## Katkıda Bulunma

Organizasyon genelindeki geliştirme kuralları, branch isimlendirme, commit formatı ve PR iş akışı için:

👉 [**CONTRIBUTING.md**](CONTRIBUTING.md)

---

## Takım Yapısı

| Takım | Alan | Açıklama |
|-------|------|----------|
| **TUFAN** | Elektromobil | Elektrikli araç tasarımı ve geliştirme |
| **LİKYA** | Otonom Araç | TUFAN bünyesinde otonom sürüş çalışmaları |

---

*Bu repo geliştirme aşamasındadır. Yeni iş akışları ve şablonlar eklendikçe bu doküman güncellenecektir.*
