# Web Sunucu Log Analizi ile DDoS / Anomali Tespiti

Bu proje, sentetik web sunucu loglarını (Apache/Nginx formatına benzer) analiz ederek:
- Yüksek trafik hacmine bağlı DDoS adaylarını
- 404 brute force denemelerini
- 3-sigma kuralı ile yüksek gecikme (response time) anomalilerini

tespit etmeyi gösterir.

## Kullanılan Teknolojiler
- Python, Jupyter Notebook
- NumPy, Pandas
- Matplotlib

## Çalıştırma
1) Ortamı kur:
   ```bash
   pip install -r requirements.txt
   ```
2) Notebook’u aç:
   ```bash
   jupyter notebook notebooks/ddos_log_anomaly_analysis.ipynb
   ```
3) Hücreleri sırayla çalıştır. Sentetik log üretilir, parse edilir ve analiz/grafikler yapılır.

## Dosya Yapısı
- `notebooks/ddos_log_anomaly_analysis.ipynb`: Tüm analiz akışı
- `requirements.txt`: Bağımlılıklar
- `data/` (isteğe bağlı): Gerçek log dosyaları için klasör (büyük dosyaları repoya eklemeyin, .gitignore’a ekleyin)
