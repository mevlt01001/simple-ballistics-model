# Mermi Yörüngesi ve Penetrasyon Simülasyonu

Bu proje, mermilerin aerodinamik özelliklerini ve hedefe çarpışma anındaki etkilerini modelleyen başlangıç seviyesinde bir balistik simülasyondur. **Gerçek hayattaki balistik olayları tam olarak yansıtmaz**, ancak temel fiziksel kavramları anlamak ve modellemek için iyi bir uygulama sunar.

---

## Kapsam ve Amaç
- Farklı mermi ve hedef türlerinin uçuş dinamikleri üzerinde nasıl etki gösterdiğini incelemek.
- **Merminin yörüngesi, sürüklenme kuvveti ve kinetik enerjisinin** hedef üzerindeki etkilerini modellemek.
- **Euler yöntemi** ile basit yörünge simülasyonu gerçekleştirmek.
- **Hedef malzemeleri ile merminin penetrasyon derinliği ve deformasyon çapını** hesaplamak.

Bu simülasyon; **fizik, mühendislik ve balistik alanlarına ilgi duyan** öğrenciler ve araştırmacılar için temel bir eğitim aracı olmayı amaçlar.


---

## Varsayımlar ve Sınırlar
1. **Çevresel Faktörlerin Sınırlı Modellenmesi:**  
   - Hava yoğunluğu, nem ve sıcaklık gibi çevresel parametreler modele dahil edilmiştir, ancak **rüzgar ve atmosfer basıncı değişimleri** dikkate alınmamıştır.  
   - **Yerçekimi ivmesi (9.81 m/s²)** sabit kabul edilmiştir ve değişken araziler göz önünde bulundurulmamıştır.

2. **Sabit Hedef Özellikleri:**  
   - Çarpma sonrası oluşan hasar yalnızca **plastik deformasyon** ve penetrasyon derinliği ile sınırlandırılmıştır.
   - Hedef malzemesinin **homojen** olduğu varsayılır (örneğin, çelik veya beton malzemenin her noktasının aynı özelliklere sahip olduğu kabul edilir).

3. **Mermi Modeli:**  
   - Mermiler sadece **rijit cisimler** olarak ele alınır, dolayısıyla esneme veya şekil değişiklikleri göz önünde bulundurulmamıştır.
   - Merminin **dönme hareketi** (spin) veya savrulma etkileri dikkate alınmamıştır.

4. **Basitleştirilmiş Aerodinamik Model:**  
   - Sürüklenme katsayısı (Cd), **Mach sayısı ve Reynolds sayısına** göre dinamik olarak değişir. Ancak daha karmaşık akış etkileri (örneğin şok dalgaları) modele dahil edilmemiştir.
   - **Süpersonik ve transsonik rejimler** için katsayılar basit regresyonlarla modellenmiştir.

5. **Enerji Kaybı Hesapları:**  
   - Mermi-çarpma anında enerji kaybı **tam elastik olmayan çarpışma** varsayımına dayalı olarak hesaplanmıştır.  
   - Çarpışma sonrası oluşan deformasyon, sadece kinetik enerjinin bir kısmının hedef malzemeye aktarılması üzerinden değerlendirilmiştir.

6. **Hedef Mesafesi ve Uçuş Süresi:**  
   - Mermi, sabit bir başlangıç hızında fırlatılır ve **uçuş süresi boyunca hava sürtünmesi** hesaba katılır.
   - Simülasyon, merminin **hedefe ulaşana kadar yörüngesini** takip eder veya yere çarptığında durur.

---

## Kullanım Adımları
1. **Google Colab Üzerinde Çalıştırın:**  
   Proje, Google Colab üzerinde çalıştırılmak üzere tasarlanmıştır. Kütüphaneleri kurmanıza gerek yoktur. Colab üzerinden doğrudan çalıştırabilirsiniz.

2. **Özelleştirme:**  
   - Mermi türlerini, hedef malzemelerini ve başlangıç hızlarını değiştirerek farklı senaryoları inceleyebilirsiniz.
   - Çevresel parametreleri (hava yoğunluğu, nem vb.) değiştirerek simülasyonu özelleştirin.

---

## Çıktılar
- **Penetrasyon Derinliği:** Merminin hedefe ne kadar nüfuz ettiği.
- **Deformasyon Çapı:** Çarpışma sonrası hedefte oluşan çukurun çapı.
- **Yörünge Grafikleri:** Merminin uçuş sırasında izlediği yolun görselleştirilmesi.
- **Hız ve Drag Kuvveti Grafikleri:** Zaman içinde merminin hız değişimi ve sürüklenme kuvveti.

---

## Örnek Mermi Türleri
- **9mm Tabanca Mermisi**  
- **5.56 NATO Mermisi**  
- **7.62 NATO Mermisi**  
- **12.7 mm (0.50 Cal BMG)**  
- **155 mm Top Mermisi**

## Örnek Hedef Türleri
- **Çelik**  
- **Alüminyum**  
- **Tungsten**  
- **Beton**  
- **Kevlar**

---

## Lisans
Bu proje açık kaynak olarak paylaşılmaktadır. Projeyi kullanabilir, geliştirebilir veya üzerinde değişiklikler yapabilirsiniz.

