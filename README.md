# AutoSurvey

**AutoSurvey**, Python ile anket verilerini otomatik olarak analiz etmeye yarayan açık kaynak bir kütüphanedir. Kullanıcıdan alınan anket verileri üzerinde temel istatistiksel analizler yapar ve görselleştirmelerle destekler.

##  Özellikler

- Frekans analizleri
- Çapraz tablolar (crosstab)
- Ortalama, standart sapma hesaplama
- Hipotez testleri (t-testi, ki-kare)
- Otomatik grafik üretimi (bar chart, heatmap vs.)
- Kullanıcı dostu arayüz (isteğe bağlı Streamlit)

##  Kullanım Örneği

```python
from autosurvey import SurveyAnalyzer

analyzer = SurveyAnalyzer("data/example_survey.csv")
analyzer.frequency("gender")
analyzer.crosstab("gender", "education_level")
analyzer.plot_bar("age_group")
```

##  Kullanılan Teknolojiler

- Python
- Pandas
- Statsmodels
- SciPy
- Matplotlib / Seaborn
- (Opsiyonel) Streamlit

##  Amaç

Bu proje, araştırmacıların veya veri analizine yeni başlayan kullanıcıların, anket verileri ile hızlı ve doğru analizler yapabilmelerini sağlamayı hedefler.

## Örnek Veri

`data/` klasörüne örnek bir `.csv` dosyası yükleyerek analizleri başlatabilirsiniz.

## Geliştirici

Proje: Google Summer of Code 2025 kapsamında Python Software Foundation için önerilmiştir.  
Geliştirici: [@cansualltnts](https://github.com/cansualltnts)
