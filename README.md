# Proteus NTC ve PTC Devresi (Proteus #6)


🔗 [Web Siteme Bakmak İçin Tıkla](https://www.hakkiharmankaya.com/)

Proteus'ta sıcaklığa duyarlı NTC (Negatif Sıcaklık Katsayısı) ve PTC (Pozitif Sıcaklık Katsayısı) termistörlerini kullanarak ışık kontrollü iki farklı devre tasarlayabilirsin. Bu devreler, sıcaklık değişimlerine bağlı olarak transistörleri tetikleyerek LED’in yanmasını veya sönmesini sağlar.

---

## 🔧 Gerekli Malzemeler

- NTC Termistör  
- PTC Termistör  
- NPN Transistör (BC547)  
- LED  
- Direnç (1kΩ, 10kΩ)  
- DC Güç Kaynağı (5V)  
- Proteus Simülasyon Yazılımı

---

## 🔬 NTC Termistör Devresi

### 🛠️ Devre Kurulumu

1. Proteus'ta bileşenleri eklemek için "P" tuşuna bas. `NTC`, `BC547`, `LED`, `Resistor` elemanlarını projeye ekle.
2. NTC’nin bir ucunu **5V** kaynağa, diğer ucunu **10kΩ direnç** üzerinden **GND**'ye bağla.
3. Bu iki bileşenin birleşim noktasından **transistörün baz (B)** ucuna bir bağlantı yap. Araya **1kΩ direnç** ekle.
4. Transistörün **kolektör (C)** ucuna LED’in **anot** ucu bağlanır, **katot** ucuna ise doğrudan GND.
5. **Emetör (E)** ucu GND’ye bağlanır.

### 🔍 Çalışma Prensibi

- 🌡️ Sıcaklık arttıkça → **NTC’nin direnci azalır**  
- Baz akımı artar → Transistör iletime geçer → **LED yanar**  
- Sıcaklık azaldığında → Direnç artar → Transistör kesime gider → **LED söner**

---

## 🔬 PTC Termistör Devresi

### 🛠️ Devre Kurulumu

1. "P" tuşuna basarak `PTC`, `BC547`, `LED`, `Resistor` bileşenlerini ekle.
2. PTC’nin bir ucunu **5V** kaynağa, diğer ucunu **10kΩ direnç** ile GND’ye bağla.
3. Bu iki bileşenin birleşim noktasını **transistörün baz (B)** ucuna bağla. Araya yine **1kΩ direnç** koyabilirsin.
4. Kolektöre LED bağla → Katotu GND'ye. Emetör doğrudan GND’ye.

### 🔍 Çalışma Prensibi

- 🌡️ Sıcaklık arttıkça → **PTC’nin direnci artar**  
- Baz akımı azalır → Transistör kesime gider → **LED söner**  
- Sıcaklık azaldığında → Direnç düşer → Transistör iletime geçer → **LED yanar**

---

## ⚙️ Sonuç

| Devre Türü  | Sıcaklık Artınca | Sıcaklık Azalınca |
|-------------|------------------|--------------------|
| **NTC**     | LED yanar        | LED söner          |
| **PTC**     | LED söner        | LED yanar          |

Bu iki farklı termistör devresi sayesinde sıcaklık kontrollü sistemleri simüle edebilir, Proteus’ta sıcaklık sensörlerinin nasıl çalıştığını gözlemleyebilirsin.

