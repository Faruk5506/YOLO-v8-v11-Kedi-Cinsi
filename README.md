# YOLO Mimarileri ile Derin Öğrenme Tabanlı Nesne Tespiti 🚀

Bu proje, bilgisayarlı görü (computer vision) teknikleri kullanılarak özel bir veri seti üzerinde yüksek doğruluklu nesne tespiti yapabilen bir yapay zeka modelinin eğitim ve test süreçlerini içermektedir. Çalışma kapsamında endüstri standardı olan **YOLOv8** ve güncel **YOLOv11** mimarileri kullanılmış, sürümler arası performans artışı analiz edilmiştir.

## 🎯 Projenin Amacı
Projenin temel hedefi, modelin belirlenen nesneleri minimum hata payı (False Positive) ve yüksek hassasiyetle tanıyabilmesini sağlamaktır. Python tabanlı olarak geliştirilen bu sistem, hem statik görseller üzerinde hem de OpenCV entegrasyonu ile canlı kamera akışında çalışabilmektedir.

## 🛠️ Kullanılan Teknolojiler
* **Dil:** Python
* **Derin Öğrenme & Görüntü İşleme:** Ultralytics (YOLO), OpenCV
* **Veri Analizi:** Pandas
* **Geliştirme Ortamı:** Anaconda CLI

## 📊 Eğitim Süreci ve Performans Sonuçları
Model, donanım kaynakları optimize edilerek 640x640 görüntü boyutu (`imgsz=640`) ve 50 epoch parametreleriyle eğitilmiştir. İteratif geliştirme süreci sonucunda mimari güncellenmiş ve performans ciddi oranda artırılmıştır.

* **Aşama 1 (YOLOv8):** Temel eğitimler tamamlandı, %82 mAP50 ve %98 Precision değerleri elde edildi.
* **Aşama 2 (YOLOv11):** Güncel mimariye geçiş yapılarak eğitim baştan tekralandı. 

**🏆 YOLOv11 Final Başarı Metrikleri:**
* **Precision (Nokta Atışı Doğruluk):** %99 (0.990)
* **mAP50 (Genel Başarı):** %87 (0.871)

YOLOv11 mimarisine geçiş ile birlikte modelin yanılma payı neredeyse sıfıra indirilmiş ve özellik çıkarımı çok daha keskin hale getirilmiştir.

## 💻 Kurulum ve Kullanım

**1. Gerekli kütüphaneleri yükleyin:**
```bash
pip install ultralytics opencv-python pandas
