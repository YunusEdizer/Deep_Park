# Deep_Park
DeepPark
Model Uygulama ve Test Süreci (Yunus Emre Edizer)

Bu çalışmada, otopark doluluk tespiti için Leaky ReLU aktivasyon fonksiyonu ve Average Pooling katmanlarına sahip bir CNN modeli oluşturulmuş ve test edilmiştir. Uygulanan adımlar şöyledir:

Veri Ön İşleme: Veri seti ImageFolder yapısı ile okunmuş, tüm görüntüler 64x64 piksel boyutuna getirilmiş ve rastgele olarak %80 Eğitim, %20 Test verisi şeklinde ayrılmıştır.

Model Mimarisi: Modelde iki adet konvolüsyon katmanı, negatif değerlere 0.1 eğim veren Leaky ReLU ve Average Pooling (2x2) katmanları kullanılmıştır.

Eğitim Konfigürasyonu: Model, Adam optimizasyon algoritması (lr=0.001) ve CrossEntropyLoss kayıp fonksiyonu ile derlenmiştir.

Test: Model 3 epoch (dönem) boyunca eğitilmiş, her epoch sonunda eğitim kaybı ve doğruluğu ölçülmüş, son olarak ayrılan test seti üzerinde nihai başarım oranı hesaplanmıştır.
