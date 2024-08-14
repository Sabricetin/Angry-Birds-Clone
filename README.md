# Angry Birds Clone Uygulaması

Bu Swift kodları, Angry Birds Clone uygulamasının çeşitli bölümlerini oluşturan bileşenlerdir. Uygulama, kullanıcıların kuşları fırlatarak kutuları devirmelerini sağlar. Her bir kod bloğu, belirli bir işlevi yerine getirir ve birlikte çalışarak tam bir oyun deneyimi sunar.

## 1. Oyun Sahnesi (GameScene.swift)

Bu kod, oyunun temel sahnesini oluşturur ve tüm oyun mekaniğini yönetir.

### Özellikler

- **Arayüz Elemanları:**
  - `bird`: Oyuncunun kontrol ettiği kuş.
  - `boxes`: Sahnedeki kutuların listesi.
  - `scoreLabel`: Oyuncunun skorunu gösteren etiket.

### Oyun Mekanikleri

- `didMove(to:)`: Sahne yüklendiğinde çağrılır. Fiziksel dünya ayarlarını yapar ve kuş ile kutuları sahneye ekler.
- `touchesBegan(_:with:)`: Oyuncu ekrana dokunduğunda çağrılır. Kuşu fırlatmak için başlangıç pozisyonunu ayarlar.
- `touchesMoved(_:with:)`: Oyuncu ekranda parmağını hareket ettirdiğinde çağrılır. Kuşun pozisyonunu günceller.
- `touchesEnded(_:with:)`: Oyuncu parmağını ekrandan çektiğinde çağrılır. Kuşu fırlatır.
- `update(_:)`: Oyun her frame'de çağrılır. Kuşun durumu kontrol edilir ve oyun durumu güncellenir.

### Fizik ve Çarpışma

- `didBegin(_:)`: Çarpışma tespit edildiğinde çağrılır. Kuşun bir kutuya çarpması durumunda skor artırılır.

## Kodun Genel Yapısı

- **Kuş:** Oyuncunun kontrol ettiği ana karakterdir. Fiziksel özellikleri ayarlanmış ve çarpışma tespiti yapılmıştır.
- **Kutular:** Oyuncunun kuşla vurmayı hedeflediği nesnelerdir. Fiziksel özellikleri ayarlanmış ve sahneye eklenmiştir.
- **Skor:** Oyuncunun başarısını gösterir. Her çarpışma durumunda güncellenir.

![Angry-Bird-Clone](https://github.com/user-attachments/assets/0f36aa0c-7e28-4bc5-ad09-cbf3d74037ab)
