# 🧪 QA Masterclass: Test Engineering Bootcamp Ödevi
# TESTRAİL LİNKİ: https://masterclass1369.testrail.io/index.php?/dashboard

Bu proje, QA Masterclass kapsamında verilen Yazılım Test Süreçleri ödevinin kapsamlı bir şekilde uygulanmasını içermektedir. Ödev 3 temel başlıktan oluşmaktadır: **Manuel Test**, **Test Otomasyonu**, ve **API Testleri**.

📅 **Teslim Tarihi:** 04 Ağustos 2025, Saat 23:59  
📁 **Teslim Şekli:** GitHub Public Repository  
📧 **Gönderim:** Repository linki `can.sekerr@outlook.com` adresine iletilecektir.

---

## 📌 İçindekiler

- [🔍 Manuel Test](#-manuel-test)
- [🤖 Test Otomasyonu](#-test-otomasyonu)
- [🌐 API Testleri](#-api-testleri)
- [📁 Proje Yapısı](#-proje-yapısı)
- [📝 Gereksinimler](#-gereksinimler)
- [📌 Notlar](#-notlar)

---

## 🔍 Manuel Test

**Test Edilen Web Sitesi:** [https://www.trendyol.com](https://www.trendyol.com)

### ✔️ Hazırlanan Senaryolar

- Ürün detay sayfası görüntülenmesi
- Ürün sepete eklenmesi
- Sepette ürün bilgisi kontrolü
- Fiyat filtresi testi
- Favorilere ürün ekleme
- Giriş işlemi
- Kategori filtresi
- Sepetteki ürün adedi artırma
- Hediye paketi seçeneği
- Sepet boşken uyarı mesajı

### 📄 Belgeler

- `ManualTestCases.xlsx`: Tüm senaryoların detaylı test adımlarını, beklenen-sonuç ilişkisini ve test durumunu içerir.
- `BugReports.xlsx`: Testler sırasında tespit edilen hataların her biri için oluşturulan bug raporlarını içerir. Her raporda adım adım nasıl yeniden üretileceği ve ekran görüntüsü mevcuttur.

---

## 🤖 Test Otomasyonu

**Araçlar:**
- Selenium WebDriver
- NUnit
- C#
- ChromeDriver
- Extent Reports

### 🔧 Otomatize Edilen Senaryolar

- Ürün detay sayfası açılıyor mu?
- Ürün sepete eklenebiliyor mu?
- Sepet sayfası ürün bilgilerini gösteriyor mu?
- Sepetteki ürün silinebiliyor mu?
- Fiyat filtresi çalışıyor mu?
- Ürün sıralama (En Düşük Fiyat) doğru mu?

### 🤖 Otomasyon Testi

- <img width="1887" height="912" alt="TestRail1" src="https://github.com/user-attachments/assets/22cefed7-9d96-499b-97c8-373838ef8f10" />
<img width="1900" height="925" alt="TestRail2" src="https://github.com/user-attachments/assets/496bfb31-b6b9-4c0b-a7cc-ccf105650d74" />
<img width="1914" height="925" alt="TestRail3" src="https://github.com/user-attachments/assets/d028d591-b6f6-46f4-a707-448acfe17a6e" />
<img width="1914" height="925" alt="TestRail4" src="https://github.com/user-attachments/assets/2dcbb7e0-9137-4e51-a303-0dffe5039451" />
<img width="1916" height="925" alt="TestRail5" src="https://github.com/user-attachments/assets/4f1d2657-fdfd-4aaa-8dcd-4353ff877f07" />
<img width="1910" height="908" alt="TestRail6" src="https://github.com/user-attachments/assets/d691a09b-89c9-4b9f-a23e-8ffd51c0ed36" />
  
## Test Case 1: Arama kutusu çalışıyor mu?

**Preconditions:**  
Kullanıcı Trendyol ana sayfasında olmalı.

**Steps:**  
1. Ana sayfada yer alan arama kutusuna “ayakkabı” yazılır.  
2. Klavyeden Enter tuşuna basılır.  

**Expected Result:**  
Ürün arama sonuç sayfası yüklenir ve ayakkabılar listelenir.

**Priority:** High  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 2: Ürün detay sayfası açılıyor mu?

**Preconditions:**  
Kullanıcı ürün arama sayfasında olmalı.

**Steps:**  
1. Listelenen ürünlerden biri seçilir.  
2. Ürün görseline veya adına tıklanır.  

**Expected Result:**  
Ürün detay sayfası açılır.

**Priority:** High  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 3: Ürün sepete eklenebiliyor mu?

**Preconditions:**  
Kullanıcı ürün detay sayfasında olmalı.

**Steps:**  
1. “Sepete Ekle” butonuna tıklanır.  

**Expected Result:**  
Ürün sepete başarıyla eklenir ve bildirim gösterilir.

**Priority:** High  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 4: Sepet sayfası ürün bilgilerini gösteriyor mu?

**Preconditions:**  
Kullanıcının sepetinde en az 1 ürün olmalı.

**Steps:**  
1. Sepet ikonuna tıklanır.  
2. Sepet sayfası açılır.  

**Expected Result:**  
Ürün adı, fiyatı ve adedi gibi bilgiler doğru şekilde listelenir.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 5: Sepetteki ürün silinebiliyor mu?

**Preconditions:**  
Sepette en az 1 ürün bulunmalı.

**Steps:**  
1. Sepetteki ürünün yanındaki “Sil” butonuna tıklanır.  

**Expected Result:**  
Ürün sepetten kaldırılır.

**Priority:** High  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 6: Fiyat filtresi çalışıyor mu?

**Preconditions:**  
Kullanıcı filtreli ürün kategorisinde olmalı.

**Steps:**  
1. Minimum ve maksimum fiyat değerleri girilir.  
2. “Uygula” butonuna tıklanır.  

**Expected Result:**  
Listelenen ürünler belirtilen fiyat aralığına uygundur.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 7: Ürün sıralama (En Düşük Fiyat) doğru mu?

**Preconditions:**  
Kullanıcı bir kategori sayfasında olmalı.

**Steps:**  
1. “Sırala” menüsünden “En Düşük Fiyat” seçeneği tıklanır.  

**Expected Result:**  
Ürünler artan fiyat sırasına göre listelenir.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 8: Kullanıcı hesabına giriş yapılabiliyor mu?

**Preconditions:**  
Kullanıcı Trendyol ana sayfasında olmalı.

**Steps:**  
1. “Giriş Yap” butonuna tıklanır.  
2. E-posta ve şifre girilir.  
3. “Giriş Yap” butonuna tekrar tıklanır.  

**Expected Result:**  
Kullanıcı hesabına başarılı şekilde giriş yapılır.

**Priority:** High  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 9: Favorilere ürün eklenebiliyor mu?

**Preconditions:**  
Kullanıcı giriş yapmış olmalı.

**Steps:**  
1. Bir ürünün kalp ikonuna tıklanır.  

**Expected Result:**  
Ürün favorilere eklenir.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 10: Sepetteki ürün adedi artırılabiliyor mu?

**Preconditions:**  
Sepette ürün bulunmalı.

**Steps:**  
1. Ürün yanındaki adet artırma butonuna (+) tıklanır.  

**Expected Result:**  
Ürün adedi 1 artar.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 11: Ürün yorumları görüntülenebiliyor mu?

**Preconditions:**  
Kullanıcı ürün detay sayfasında olmalı.

**Steps:**  
1. Sayfa aşağıya kaydırılır.  
2. “Yorumlar” sekmesi tıklanır.  

**Expected Result:**  
Ürünle ilgili kullanıcı yorumları listelenir.

**Priority:** Low  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 12: Kategoriler menüsü çalışıyor mu?

**Preconditions:**  
Kullanıcı ana sayfada olmalı.

**Steps:**  
1. Sayfa üstündeki “Kategoriler” menüsüne tıklanır.  
2. Herhangi bir alt kategori seçilir.  

**Expected Result:**  
Seçilen kategoriye ait ürünler listelenir.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 13: Sepet boşken uyarı mesajı gösteriliyor mu?

**Preconditions:**  
Sepet boş olmalı.

**Steps:**  
1. Sepet sayfasına gidilir.  

**Expected Result:**  
“Kullanıcı sepetiniz şu anda boş” mesajı görünür.

**Priority:** Low  
**Type:** UI  
**Template:** Test Case (Steps)

---

## Test Case 14: Mobil görünümde menü açılıyor mu?

**Preconditions:**  
Kullanıcı mobil tarayıcıdan giriş yapmış olmalı.

**Steps:**  
1. Üst menüdeki hamburger ikonuna tıklanır.  

**Expected Result:**  
Menü öğeleri mobilde görünür hale gelir.

**Priority:** Medium  
**Type:** UI/Responsive  
**Template:** Test Case (Steps)

---

## Test Case 15: Hediye paketi seçeneği çalışıyor mu?

**Preconditions:**  
Kullanıcı ürün detay sayfasında olmalı.

**Steps:**  
1. “Hediye paketi” seçeneği işaretlenir.  
2. Sepet sayfasına gidilir.  

**Expected Result:**  
Sepette ürünün yanında hediye paketi seçildiği görünür.

**Priority:** Low  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 16: Yukarı çık butonu

**Preconditions:**  
Sayfa en az 2 ekran uzunluğunda kaydırılmış olmalı.

**Steps:**  
1. Sayfa en altına inilir.  
2. Sağ altta çıkan yukarı ok ikonuna tıklanır.  

**Expected Result:**  
Sayfa en üst kısmına kayar.

**Priority:** Low  
**Type:** UI  
**Template:** Test Case (Steps)

---

## Test Case 17: İndirim kuponu

**Preconditions:**  
Kullanıcının kullanabileceği kupon olmalı.

**Steps:**  
1. Sepete ürün eklenir.  
2. Sepette “Kupon Ekle” alanına indirim kodu girilir.  

**Expected Result:**  
İndirim uygulanır ve toplam tutar azalır.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 18: Ürün karşılaştırma özelliği çalışıyor mu?

**Preconditions:**  
Kullanıcı kategori sayfasında olmalı.

**Steps:**  
1. En az iki ürün karşılaştırma kutucuğu seçilir.  
2. “Karşılaştır” butonuna tıklanır.  

**Expected Result:**  
Seçilen ürünler karşılaştırma tablosunda listelenir.

**Priority:** Low  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 19: Kargo bilgisi görüntülenebiliyor mu?

**Preconditions:**  
Kullanıcı ürün detay sayfasında olmalı.

**Steps:**  
1. “Kargo Bilgisi” sekmesine tıklanır.  

**Expected Result:**  
Tahmini teslimat tarihi ve kargo ücret bilgisi görünür.

**Priority:** Medium  
**Type:** Functional  
**Template:** Test Case (Steps)

---

## Test Case 20: İndirimli ürünler doğru şekilde etiketleniyor mu?

**Preconditions:**  
Kullanıcı ana sayfada olmalı.

**Steps:**  
1. Ürün listesi incelenir.  
2. Etiketli ürünler kontrol edilir.  

**Expected Result:**  
İndirimli ürünler üzerinde “İndirim” veya yüzdelik etiket görünür.

**Priority:** Low  
**Type:** UI  
**Template:** Test Case (Steps)

---
### 🧪 Manuel Testler

- Test Case Excel Görüntüsü  
  !(<img width="1772" height="775" alt="TestSenaryoları" src="https://github.com/user-attachments/assets/a2233e67-73c0-4e7f-bb1f-9082be7b5db0" />
)

- Hata Raporları  
  !<img width="1655" height="775" alt="BugRaporu" src="https://github.com/user-attachments/assets/d4760c18-6ad8-4772-b6a3-9c1a56be82ab" />
[testrail-report-2-standalone.zip](https://github.com/user-attachments/files/21530778/testrail-report-2-standalone.zip)
 
[testrail-report-1.pdf](https://github.com/user-attachments/files/21530628/testrail-report-1.pdf)

[testrail-report-2.pdf](https://github.com/user-attachments/files/21530627/testrail-report-2.pdf)

### 🌐 API Testleri

- Postman Collection Görünümü  
PetStore.postman_collection_EdaOzgeUgurlu

  ## 💬 Katkı ve Geri Bildirim

Bu ödev QA Masterclass eğitim programı kapsamında bireysel olarak hazırlanmıştır. Görüş, öneri veya geri bildirimlerinizi memnuniyetle karşılarım.

📧 E-posta: edaozgeugurlu@gmail.com  
🔗 LinkedIn[: [https://www.linkedin.com/in/edaozgeugurlu/]


