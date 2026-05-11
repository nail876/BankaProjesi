# 🏦 Banka Yönetim Sistemi Simülasyonu

[cite_start]Bursa Teknik Üniversitesi, Bilgisayar Mühendisliği Bölümü **BLM0121 Nesneyi Yönelik Programlama** dersi proje ödevi kapsamında geliştirilmiştir[cite: 3, 4]. Uygulama; müşteri yönetimi, hesap işlemleri ve kredi kartı süreçlerini kapsayan modüler bir bankacılık simülasyonudur.

## 👤 Geliştirici Bilgileri
* [cite_start]**Ad Soyad:** Nail Buğra Önür [cite: 10, 11]
* [cite_start]**Öğrenci No:** 24360859010 [cite: 10, 11]
* [cite_start]**Üniversite:** Bursa Teknik Üniversitesi (BTÜ) [cite: 2]
* [cite_start]**Bölüm:** Bilgisayar Mühendisliği [cite: 3]

---

## 🚀 Proje Özeti
[cite_start]Bu proje; müşteri, banka personeli, hesap türleri ve kredi kartları arasındaki ilişkileri gerçek dünya mantığına uygun bir şekilde modeller[cite: 21, 22]. [cite_start]Projenin temel odağı, karmaşık finansal süreçleri **Nesne Yönelimli Programlama** disipliniyle (Inheritance, Polymorphism, Abstraction, Encapsulation) çözerek sürdürülebilir bir yazılım mimarisi oluşturmaktır[cite: 39, 40].

## 🛠️ Teknik Mimari ve Uygulanan Prensipler
[cite_start]Sistem, proje dökümanında belirtilen zorunlu paket hiyerarşisi üzerine inşa edilmiştir[cite: 38, 40]:

* [cite_start]**Otomatik Veri Üretimi:** PersonelID, musteriNumarasi, kartNumarasi ve IBAN değerleri, `Random` sınıfı kullanılarak sistem tarafından otomatik olarak üretilir[cite: 36].
* [cite_start]**Soyutlama ve Kalıtım:** `Kisi` ve `BankaHesabi` sınıfları temel alınarak `BankaPersoneli`, `Musteri`, `VadesizHesap` ve `YatirimHesabi` sınıfları arasında güçlü bir kalıtım yapısı kurulmuştur[cite: 22, 55, 85].
* [cite_start]**Dinamik Veri Yönetimi:** Müşteri listeleri, banka hesapları ve kredi kartları `ArrayList` yapısı ile dinamik olarak yönetilir[cite: 23, 24].
* [cite_start]**Encapsulation (Kapsülleme):** Tüm kritik veriler `private` erişim belirleyicileri ile korunmuş, verilere erişim kontrollü `getter/setter` metodları üzerinden sağlanmıştır[cite: 35].

## 📂 Paket ve Sınıf Yapısı
[cite_start]Proje, dökümanda belirtilen 5 paket altında organize edilmiştir[cite: 40]:

* [cite_start]**`com.bank.app.people`**: `Kisi`, `Musteri` ve `BankaPersoneli` sınıflarını içerir[cite: 41].
* [cite_start]**`com.bank.app.accounts`**: `BankaHesabi`, `VadesizHesap` ve `YatirimHesabi` sınıflarını içerir[cite: 42].
* [cite_start]**`com.bank.app.cards`**: `KrediKarti` sınıfını içerir[cite: 43].
* [cite_start]**`com.bank.app.service`**: İş mantığını gerçekleştiren `BankaService` sınıfını içerir[cite: 44].
* [cite_start]**`com.bank.app.main`**: Uygulamanın başlangıç noktası olan `Main` sınıfını içerir[cite: 45].

## 💻 Çalıştırma Talimatları
Projeyi yerel makinenizde derlemek ve çalıştırmak için:

1. Terminal üzerinden `src` klasörüne gidin:
   ```bash
   cd BankaProjesi/src
