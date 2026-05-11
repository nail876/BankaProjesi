# 🏦 Banka Yönetim Sistemi Simülasyonu

Bursa Teknik Üniversitesi, Bilgisayar Mühendisliği Bölümü **BLM0121 Nesneyi Yönelik Programlama** dersi proje ödevi kapsamında geliştirilmiştir. Uygulama; müşteri yönetimi, hesap işlemleri ve kredi kartı süreçlerini kapsayan modüler bir bankacılık simülasyonudur.

## 👤 Geliştirici Bilgileri
**Ad Soyad:** Nail Buğra Önür 
**Öğrenci No:** 24360859010 
**Üniversite:** Bursa Teknik Üniversitesi (BTÜ) 
**Bölüm:** Bilgisayar Mühendisliği 

---

## 🚀 Proje Özeti
Bu proje; müşteri, banka personeli, hesap türleri ve kredi kartları arasındaki ilişkileri gerçek dünya mantığına uygun bir şekilde modeller. Projenin temel odağı, karmaşık finansal süreçleri **Nesne Yönelimli Programlama** disipliniyle (Inheritance, Polymorphism, Abstraction, Encapsulation) çözerek sürdürülebilir bir yazılım mimarisi oluşturmaktır.

## 🛠️ Teknik Mimari ve Uygulanan Prensipler
Sistem, proje dökümanında belirtilen zorunlu paket hiyerarşisi üzerine inşa edilmiştir:

**Otomatik Veri Üretimi:** PersonelID, musteriNumarasi, kartNumarasi ve IBAN değerleri, `Random` sınıfı kullanılarak sistem tarafından otomatik olarak üretilir.
**Soyutlama ve Kalıtım:** `Kisi` ve `BankaHesabi` sınıfları temel alınarak `BankaPersoneli`, `Musteri`, `VadesizHesap` ve `YatirimHesabi` sınıfları arasında güçlü bir kalıtım yapısı kurulmuştur.
**Dinamik Veri Yönetimi:** Müşteri listeleri, banka hesapları ve kredi kartları `ArrayList` yapısı ile dinamik olarak yönetilir.
**Encapsulation (Kapsülleme):** Tüm kritik veriler `private` erişim belirleyicileri ile korunmuş, verilere erişim kontrollü `getter/setter` metodları üzerinden sağlanmıştır.

## 📂 Paket ve Sınıf Yapısı
Proje, dökümanda belirtilen 5 paket altında organize edilmiştir:

**`com.bank.app.people`**: `Kisi`, `Musteri` ve `BankaPersoneli` sınıflarını içerir.
**`com.bank.app.accounts`**: `BankaHesabi`, `VadesizHesap` ve `YatirimHesabi` sınıflarını içerir.
**`com.bank.app.cards`**: `KrediKarti` sınıfını içerir.
**`com.bank.app.service`**: İş mantığını gerçekleştiren `BankaService` sınıfını içerir.
**`com.bank.app.main`**: Uygulamanın başlangıç noktası olan `Main` sınıfını içerir.

## 💻 Çalıştırma Talimatları
Projeyi yerel makinenizde derlemek ve çalıştırmak için:

1. Terminal üzerinden `src` klasörüne gidin:
   ```bash
   cd BankaProjesi/src
