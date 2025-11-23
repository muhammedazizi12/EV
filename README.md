EV Charging Security — OCPP & Yapay Zekâ Destekli Anomali Tespiti


📌 Projenin Özeti

Bu proje, elektrikli araç şarj istasyonlarında gerçekleşen enerji akışını gerçek zamanlı olarak izleyerek olağandışı davranışları (anomali) tespit eden güvenlik odaklı bir simülasyon sistemidir. Sistem, hem kural tabanlı hem de makine öğrenimi tabanlı yöntemleri kullanarak şüpheli durumları algılar ve kaydeder.


🎯 Amacı / Çözdüğü Problem
Şarj sürecinde ortaya çıkabilecek anormal enerji kullanımı, OCPP bağlantısı kesikken şarjın devam etmesi, negatif enerji, replay manipülasyonu gibi saldırı senaryolarını algılamak ve güvenlik risklerini azaltmak.


🔧 Projenin Özellikleri
Gerçek zamanlı enerji akışı simülasyonu
OCPP bağlantı durumu kontrolü
Kural tabanlı anomali tespiti
ML (Isolation Forest) ile anomali tespiti
Replay veri oynatma
CSV / JSON log kaydı
Renkli log görüntüleme
Kullanıcı dostu arayüz (Tkinter)


📂 Proje Dosya Yapısı
main.py
simulator.py
ml_detector.py
trainer.py
replay.py
/data
    normal_data.csv
    model.joblib
/logs
    logs.csv
README.md


▶️ Çalıştırma Talimatları

Ortam Hazırlığı:
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt

Model Eğitme (Gerekirse):
python trainer.py

Simülasyonu Başlatma:
python main.py


📦 Kullanılan Kütüphaneler
tkinter
random
datetime
csv
json
os
joblib
sklearn
numpy
pandas


