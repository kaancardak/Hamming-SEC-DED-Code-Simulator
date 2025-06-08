# 🔐 Hamming SEC-DED Kodu Simülatörü

## 📋 Proje Hakkında

Bu proje, bilgisayar mimarisi dersi kapsamında geliştirilmiş bir **Hamming SEC-DED (Single-Error-Correcting, Double-Error-Detecting)** kod simülatörüdür. Web tabanlı interaktif bir arayüz ile Hamming kodlarının nasıl çalıştığını görsel olarak öğrenmenizi sağlar.

## ✨ Özellikler

### 🎯 Temel Fonksiyonlar
- **Veri Kodlama**: 8, 16 veya 32 bitlik binary veriyi Hamming SEC-DED koduna çevirir
- **Hata Oluşturma**: Rastgele veya manuel hata ekleme
- **Hata Tespiti**: Tek ve çift bit hatalarının tespiti
- **Hata Düzeltme**: Tek bit hatalarının otomatik düzeltilmesi
- **Görselleştirme**: Bit analizi ve bellek simülasyonu

### 🎨 Kullanıcı Arayüzü
- Modern ve responsive tasarım
- Renk kodlu bit analizi (Parity, Data, Error bitleri)
- Gerçek zamanlı bildirimler
- Detaylı işlem logları
- Animasyonlu hata göstergeleri

### 🔧 Teknik Özellikler
- Vanilla JavaScript (framework dependency yok)
- CSS3 animasyonları ve gradyanlar
- Responsive mobile-first tasarım
- Ses efektleri ve görsel geri bildirimler

## 🚀 Kullanım

### Adım 1: Veri Girişi
1. "Binary Veri" alanına 8, 16 veya 32 bitlik binary kod girin
   - Örnek: `10110101` (8 bit)
   - Örnek: `1011010110110101` (16 bit)

### Adım 2: Kodlama
2. "Kodla ve Belleğe Yaz" butonuna tıklayın
   - Hamming parity bitleri otomatik hesaplanır
   - Genel parity bit eklenir (SEC-DED için)
   - Kodlanmış veri bellek simülasyonunda görüntülenir

### Adım 3: Hata Oluşturma
3. Hata oluşturma seçeneklerinden birini seçin:
   - **Rastgele Hata**: Otomatik rastgele pozisyonda hata
   - **Manuel Hata**: Belirttiğiniz pozisyonda hata

### Adım 4: Kontrol ve Düzeltme
4. "Kontrol Et ve Düzelt" butonuna tıklayın
   - Tek bit hataları tespit edilir ve düzeltilir
   - Çift bit hataları tespit edilir (düzeltilmez)
   - Hata yoksa başarı mesajı görüntülenir

## 🛠️ Teknik Detaylar

### Hamming Kodu Algoritması
- **Parity Bit Hesaplama**: `r ≥ log₂(m + r + 1)` formülü
- **Bit Yerleştirme**: 2'nin kuvvetleri pozisyonlarında parity bitleri
- **Syndrome Hesaplama**: XOR işlemleri ile hata pozisyonu tespiti
- **SEC-DED**: Genel parity bit ile çift hata tespiti

### Desteklenen Veri Boyutları
| Veri Boyutu | Parity Bit | Toplam Bit | Genel Parity | Final Boyut |
|-------------|------------|-------------|---------------|-------------|
| 8 bit       | 4 bit      | 12 bit      | 1 bit         | 13 bit      |
| 16 bit      | 5 bit      | 21 bit      | 1 bit         | 22 bit      |
| 32 bit      | 6 bit      | 38 bit      | 1 bit         | 39 bit      |


## 💻 Kurulum ve Çalıştırma

### Gereksinimler
- Modern web tarayıcısı (Chrome, Firefox, Safari, Edge)
- JavaScript desteği

### Çalıştırma
1. Repository'yi klonlayın:
   ```bash
   git clone https://github.com/kaancardak/Hamming-SEC-DED-Code-Simulator.git
   ```

2. Proje klasörüne gidin:
   ```bash
   cd Hamming-SEC-DED-Code-Simulator
   ```

3. `main.html` dosyasını web tarayıcısında açın
   - Çift tıklayın veya
   - Tarayıcıya sürükleyin veya
   - Live Server kullanın (VS Code extension)

## 🎓 Eğitim Amaçları

Bu simülatör şu konuları öğrenmenize yardımcı olur:

- **Hata Kontrolü ve Düzeltme Kodları**
- **Hamming Mesafe Kavramı**
- **Parity Bit Hesaplama Yöntemleri**
- **Binary Sistem ve Bit Manipülasyonu**
- **Bilgisayar Bellek Sistemleri**
- **SEC-DED Kodlarının Avantajları**

## 📊 Örnekleme Senaryoları

### Örnek 1: 8-bit Veri
```
Orijinal: 10110101
Kodlanmış: 1001101100101 (13 bit)
Hata sonrası: 1001101110101 (bit 7 flip)
Düzeltilmiş: 1001101100101
```

### Örnek 2: Çift Hata Tespiti
```
Orijinal: 11110000
Tek hata: Tespit edilir ve düzeltilir
Çift hata: Tespit edilir ama düzeltilmez
```

## 🤝 Katkıda Bulunma

Bu proje eğitim amaçlı geliştirilmiştir. Katkılarınızı memnuniyetle karşılarım:

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request açın

## 👨‍💻 Geliştirici

**Kaan Çardak**
- 🎓 Bilgisayar Mühendisliği Öğrencisi
- 📧 E-posta: kcrdk.1@gmail.com
- 🐙 GitHub: [@kaancardak](https://github.com/kaancardak)

⭐ Bu projeyi beğendiyseniz yıldız vermeyi unutmayın!
