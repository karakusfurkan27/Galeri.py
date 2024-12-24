# Resim Galerisi Uygulaması

Bu proje, kullanıcıların bir klasördeki resimleri yükleyip görsel olarak görüntülemelerini sağlayan bir Tkinter tabanlı resim galerisi uygulamasıdır. Uygulama, kullanıcıların resimler arasında geçiş yapmalarını ve resimlerin boyutlarını ayarlamalarını sağlar.

## Özellikler

- **Klasör Seçme:** Kullanıcılar bir klasör seçebilir ve seçilen klasördeki resimler yüklenecektir.
- **Resim Görüntüleme:** Yüklenen resimler, kullanıcıya bir arayüz üzerinden gösterilir.
- **Önceki ve Sonraki Resim:** Kullanıcılar önceki ve sonraki resimler arasında geçiş yapabilir.
- **Resim Boyutlandırma:** Resimler, 600x400 boyutlarına yeniden boyutlandırılır.
- **Desteklenen Formatlar:** .png, .jpg, .jpeg, .gif ve .bmp uzantılı resimler desteklenmektedir.

## Gereksinimler

- Python 3.x
- Tkinter kütüphanesi (Python ile birlikte gelir)
- Pillow kütüphanesi (Resim işleme için)

Pillow kütüphanesini yüklemek için:
```bash
pip install pillow
```

## Kullanım

1. **Uygulamayı Başlatma:** Uygulama başlatıldığında bir pencere açılacaktır.
2. **Klasör Seçme:** "Klasör Seç" butonuna tıklayın. Ardından resimlerin bulunduğu bir klasör seçin.
3. **Resimleri Görüntüleme:** Seçilen klasördeki resimler sırasıyla gösterilecektir.
4. **Resimler Arasında Geçiş Yapma:** 
   - "Önceki" butonuna tıklayarak önceki resmi görüntüleyebilirsiniz.
   - "Sonraki" butonuna tıklayarak sonraki resmi görüntüleyebilirsiniz.

## Kullanıcı Arayüzü

- **Resim Alanı:** Seçilen resim burada gösterilir.
- **Önceki Buton:** Önceki resmi görüntülemek için tıklanır.
- **Sonraki Buton:** Sonraki resmi görüntülemek için tıklanır.
- **Klasör Seç Butonu:** Resimlerin bulunduğu klasörü seçmek için tıklanır.

## Kod Yapısı

- **`ImageGallery` sınıfı:** Bu sınıf, Tkinter arayüzü ve resim işlemlerini yönetir.
  - **`load_images`**: Klasör seçme işlemi ve resimlerin yüklenmesi işlemi yapılır.
  - **`show_image`**: Resmin ekranda görüntülenmesini sağlar.
  - **`show_next_image`** ve **`show_previous_image`**: Resimler arasında geçiş yapılmasını sağlar.
