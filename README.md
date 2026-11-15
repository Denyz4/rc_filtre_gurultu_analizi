# RC Low-Pass Filter Simulation & Noise Analysis

Bu proje, bir **RC Alçak Geçiren Filtre (Low-Pass Filter)** devresinin frekans tepkisini Python ile simüle etmek, sisteme gerçekçi Gauss gürültüsü eklemek ve istatistiksel yöntemlerle (IQR) veri temizliği ile aykırı değer (outlier) analizi yapmak amacıyla geliştirilmiştir.

## 🚀 Proje Detayları ve Özellikler
* **Frekans Taraması:** Logaritmik ölçekte (`geomspace` kullanarak) $10\text{ Hz}$ ile $100\text{ kHz}$ arasında 1000 farklı frekans noktası.
* **Devre Parametreleri:** 
  * Direnç ($R$): $1\text{ k}\Omega$
  * Kapasitör ($C$): $100\text{ nF}$
  * Giriş Gerilimi: $5\text{ V}$
* **Gürültü Enjeksiyonu:** Sinyale $20\text{ mV}$ standart sapmalı Gauss gürültüsü (`np.random.normal`) eklenerek gerçekçi ölçüm ortamı simülasyonu.
* **Veri Analizi & Outlier Tespiti:** IQR (Interquartile Range) yöntemi kullanılarak gürültü verisinden sapmaların ve aykırı değerlerin izole edilmesi.

## 🛠️ Kullanılan Teknolojiler
* **Python**
* **NumPy** (Matematiksel hesaplamalar ve gürültü üretimi)
* **Matplotlib** (Frekans tepkisi ve gürültü dağılımı görselleştirme)

## 📊 Kurulum ve Çalıştırma
Projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. Depoyu klonlayın:
   ```bash
git clone https://github.com/Denyz4/rc_filtre_gurultu_analizi.git
