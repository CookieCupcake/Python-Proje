# Python-Proje


### Yapılacaklar Listesi

### 1. Proje Temeli

- [ ]  Proje klasörünü oluştur ([`main.py`](http://main.py), [`models.py`](http://models.py), [`storage.py`](http://storage.py), [`gui.py`](http://gui.py))
- [ ]  JSON mu CSV mi kullanılacağına karar ver
- [ ]  Örnek veri dosyası oluştur (`data.json` veya `data.csv`)

### 2. Veri Yapısı ve Dosya İşlemleri

- [ ]  Araç için veri modeli tasarla (dictionary veya `Car` sınıfı)
    - [ ]  `plaka`, `marka`, `model`, `ucret`, `durum`, `kiralayan`, `baslangic_tarihi`, `bitis_tarihi`
- [ ]  Araç listesini JSON/CSV’ye kaydeden fonksiyonu yaz
- [ ]  Uygulama açıldığında dosyadan verileri okuyan fonksiyonu yaz
- [ ]  Dosya yoksa ilk çalıştırmada otomatik oluşturma kontrolü ekle

### 3. GUI Tasarımı (Tkinter veya PyQt5)

- [ ]  Ana pencereyi oluştur
- [ ]  Araç listesi tablosunu oluştur (Plaka, Marka, Model, Günlük Ücret, Durum)
- [ ]  Yeni araç ekleme formunu tasarla (Plaka, Marka, Model, Günlük Ücret, Durum)
- [ ]  İşlem butonlarını ekle:
    - [ ]  "Araç Ekle"
    - [ ]  "Kiralama Başlat"
    - [ ]  "Aracı İade Et"
    - [ ]  "Sil"
    - [ ]  (İsteğe bağlı) "Düzenle"
    - [ ]  (İsteğe bağlı) "Verileri Kaydet"
- [ ]  (İsteğe bağlı) Arama / filtreleme alanı ekle (durum, marka/model)

### 4. Araç Ekleme İşlevi

- [ ]  Form alanlarından verileri al
- [ ]  Zorunlu alan kontrolü yap (boş alan var mı?)
- [ ]  Günlük ücretin sayısal olup olmadığını kontrol et
- [ ]  Yeni aracı listeye ekle
- [ ]  Listeyi GUI üzerinde güncelle
- [ ]  Değişiklikleri dosyaya kaydet
- [ ]  Başarılı işlem mesajı göster ("Araç başarıyla eklendi.")

### 5. Araç Listeleme ve Güncelleme

- [ ]  Dosyadan yüklenen araçları GUI tablosuna aktar
- [ ]  Yeni araç eklendiğinde tabloyu tazele
- [ ]  Silme / düzenleme sonrası tabloyu tazele

### 6. Araç Kiralama İşlemi

- [ ]  Listeden bir araç seçildi mi kontrol et
- [ ]  Kiralama formu aç (müşteri adı, başlangıç ve bitiş tarihi)
- [ ]  Tarih formatını doğrula
- [ ]  Bitiş tarihi başlangıçtan önce mi kontrol et
- [ ]  Gün sayısını hesapla
- [ ]  Toplam ücreti hesapla (gün × günlük ücret)
- [ ]  Aracın durumunu "kirada" yap
- [ ]  Kiralayan, başlangıç ve bitiş tarihlerini kaydet
- [ ]  Listeyi ve dosyayı güncelle
- [ ]  Bilgilendirme mesajı göster ("Kiralama işlemi tamamlandı.")

### 7. Araç İade İşlemi

- [ ]  Seçilen aracın "kirada" durumda olduğunu kontrol et
- [ ]  İade işlemini yap, durumu "müsait" yap
- [ ]  İade tarihini isteğe bağlı kaydet
- [ ]  (İsteğe bağlı) Kiralama geçmişi listesine kayıt ekle
- [ ]  Listeyi ve dosyayı güncelle

### 8. Araç Silme ve Düzenleme

- [ ]  Listeden bir araç seçildi mi kontrol et
- [ ]  Silme için onay penceresi göster
- [ ]  Onay verilirse aracı listeden ve dosyadan kaldır
- [ ]  (İsteğe bağlı) Düzenleme ekranı tasarla (ücret, model, durum güncelleme)
- [ ]  Listeyi ve dosyayı tekrar kaydet

### 9. Uygulama Kapatma ve Veri Kaydı

- [ ]  Uygulama kapanırken otomatik kaydetme fonksiyonunu çağır
- [ ]  "Verileri Kaydet" butonunu dosya yazma fonksiyonuna bağla
- [ ]  Program açıldığında önceki kayıtları otomatik yükle

### 10. Hata Yönetimi ve Doğrulama

- [ ]  Boş alan kontrollerini tüm formlara ekle
- [ ]  Sayısal alanlar için tip kontrolü ekle (günlük ücret, gün sayısı)
- [ ]  Tarih validasyonu ekle (format ve başlangıç–bitiş ilişkisi)
- [ ]  Hatalarda uygun uyarı pencereleri göster (messagebox ile)

### 11. Kullanıcı Geri Bildirimi

- [ ]  Başarılı ekleme, kiralama, iade, silme, kaydetme için bilgi mesajları
- [ ]  Hatalı girişlerde uyarı mesajları
- [ ]  Kritik işlemlerde (silme gibi) onay pencereleri

### 12. Ek Özellikler (İsteğe Bağlı)

- [ ]  Toplam gelir hesaplama fonksiyonu
- [ ]  Kirada olan araç sayısını hesaplama
- [ ]  En çok kiralanan marka istatistiği
- [ ]  Belirli tarih aralığında kiralanan araçları listeleme
- [ ]  Duruma göre filtre butonları ("Sadece kirada olanlar", "Müsait araçlar")
- [ ]  Matplotlib ile aylık kiralama sayısı grafiği
- [ ]  Matplotlib ile gelir grafiği

### 13. Kod Yapısı ve Modülerlik

- [ ]  Dosya işlemleri için ayrı modül ([`storage.py`](http://storage.py))
- [ ]  GUI için ayrı modül ([`gui.py`](http://gui.py))
- [ ]  Hesaplama ve iş mantığı için ayrı fonksiyonlar / modül ([`logic.py`](http://logic.py))
- [ ]  Ana dosyada ([`main.py`](http://main.py)) sadece ana akışı başlat

### 14. Son Kontrol ve Test

- [ ]  Farklı senaryolarla test et (boş alanlar, yanlış tarih, sayısal olmayan ücret vb.)
- [ ]  Dosya kapat/aç testleri yap (veriler kayboluyor mu kontrol et)
- [ ]  Arayüzde kullanım kolaylığını gözden geçir
- [ ]  Gerekirse arayüzü sadeleştir ve gereksiz karmaşayı kaldır