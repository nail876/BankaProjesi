# Define the content of the README.md file exactly as requested based on the provided text
readme_content = """# 🏦 Bank Management System Simulation

Bursa Teknik Üniversitesi, Bilgisayar Mühendisliği Bölümü **Nesne Yönelimli Programlama (NYP)** dersi kapsamında geliştirilen, modüler ve genişletilebilir bir bankacılık yönetim sistemi simülasyonudur.

## 👤 Geliştirici Bilgileri
* **Ad Soyad:** Nail Buğra Önür
* **Öğrenci No:** 24360859010
* **Üniversite:** Bursa Teknik Üniversitesi (BTÜ)
* **Bölüm:** Bilgisayar Mühendisliği

---

## 🚀 Proje Özeti
Bu çalışma; müşteri, hesap türleri ve kredi kartları arasındaki ilişkileri gerçek dünya mantığına uygun bir şekilde modeller. Projenin temel odağı, karmaşık finansal süreçleri **Nesne Yönelimli Programlama** disipliniyle (Inheritance, Polymorphism, Abstraction, Encapsulation) çözerek sürdürülebilir bir yazılım mimarisi oluşturmaktır.

## 🛠️ Teknik Mimari ve Uygulanan Prensipler
Sistem 5 ana paket hiyerarşisi üzerine inşa edilmiştir:

* **Otomatik Veri Üretimi:** IBAN, Müşteri Numarası ve 16 haneli Kredi Kartı numaraları sistem tarafından `Random` sınıfı kullanılarak çalışma anında (runtime) benzersiz şekilde üretilir.
* **Soyutlama ve Kalıtım:** `Kisi` ve `Hesap` sınıfları `abstract` olarak tanımlanarak güçlü bir kalıtım yapısı kurulmuştur. Bu sayede kod tekrarı önlenmiş ve modülerlik artırılmıştır.
* **Dinamik Veri Yönetimi:** Müşteri hesapları ve kart bilgileri sabit diziler yerine `ArrayList` yapısı ile yönetilerek sistemin ölçeklenebilir olması sağlanmıştır.
* **Encapsulation (Kapsülleme):** Tüm kritik veriler `private` erişim belirleyicileri ile korunmuş, verilere erişim ve veri manipülasyonu kontrollü `getter/setter` metodları üzerinden gerçekleştirilmiştir.

## 📂 Paket ve Sınıf Yapısı
Proje, mantıksal olarak ayrıştırılmış 5 paket altında toplanmıştır:

* **`com.bank.app.people`**: `Kisi` (Base), `Musteri` sınıflarını içerir.
* **`com.bank.app.accounts`**: `Hesap` (Base), `VadesizHesap`, `YatirimHesabi` sınıflarını içerir.
* **`com.bank.app.cards`**: `KrediKarti` sınıfını içerir.
* **`com.bank.app.services`**: Bankacılık operasyonel mantığını yürüten sınıflar için ayrılmıştır.
* **`com.bank.app.main`**: Sistemi ateşleyen ve test senaryolarını koşturan merkez sınıftır.

## 💻 Çalıştırma Talimatları
Projeyi yerel makinenizde derlemek ve çalıştırmak için:

1. Terminal üzerinden `src` klasörüne gidin:
