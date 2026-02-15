# Amazon Web Scraper

Amazon ürünlerini otomatik olarak çeken ve verilerini toplayan bir web scraping projesidir.

## 📋 Proje Açıklaması

Bu proje Playwright ve Bright Data kullanarak Amazon'dan ürün bilgilerini (başlık, fiyat, resim, rating vb.) scrape eder ve JSON formatında kaydeder. Scraped verileri web arayüzünde görselleştirir.

## 🛠️ Kullanılan Teknolojiler

- **Python 3.x** - Backend scraping
- **Playwright** - Web browser automation
- **Bright Data** - Proxy hizmeti
- **HTML/CSS/JavaScript** - Frontend görselleştirme

## 📦 Dosya Yapısı

```
├── main.py              # Python scraping script
├── index.html           # Ana HTML sayfası
├── script.js            # Frontend JavaScript
├── style.css            # CSS stilleri
├── scraped_data.json    # Scraped ürün verileri
└── .gitignore           # Git ignore kuralları
```

## ⚙️ Kurulum

1. Gerekli Python paketlerini yükleyin:
```bash
pip install playwright
```

2. `main.py` dosyasında Bright Data API anahtarını ekleyin:
```python
SBR_WS_CDP = "YOUR_BRIGHT_DATA_KEY_HERE"
```

## 🚀 Kullanım

Python script'ini çalıştırarak Amazon ürünlerini scrape edin:
```bash
python main.py
```

Verileri web tarayıcıda görüntülemek için `index.html`'i açın.

## 📊 Scraped Veriler

Proje aşağıdaki bilgileri toplayan her ürün için:
- **Ürün Başlığı** (title)
- **URL** (product link)
- **Resim** (image source)
- **Fiyat** (fee)
- **Rating** (user rating)

## 📝 Notlar

- Bright Data proxy hizmeti gereklidir
- Amazon'un robot kontrol sistemi (CAPTCHA vb.) etkinleştirilirse timeout alabilirsiniz
- Büyük ölçekli scraping için rate limiting yapmayı unutmayın

## 📄 Lisans

Bu proje açık kaynak kodlu, serbestçe kullanılabilir.
