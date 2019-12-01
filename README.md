# TezHaber
Turkish News Aggregator &amp; Summarizer

## Hedefimiz

Projedeki amacımız çeşitli kaynaklarda bulunan aynı bilgileri bir araya toplayıp bunları özetleyerek zaman kaybı ve yanlış bilgi edinimini engellemeyi amaçladık. Örneğin haber kaynakları, twitterdaki konular, eğitim kaynakları gibi. Bu çalışmada amacımıza yönelik olarak haber kaynaklarından aynı haberi bahseden siteleri bir araya toparlayıp özetleme işlemi gerçekleştirdik. 

## Yapılan İşlemler

- Çeşitli haber kaynaklarının RSS lerinden haberler çekilerek, json dosyası oluşturuldu
```
{
	"ahaber": {
		"rss": "https://www.ahaber.com.tr/rss/son24saat.xml",
		"link": "https://www.ahaber.com.tr/"
	},
	"aa": {
		"rss": "https://www.aa.com.tr/tr/rss/default?cat=guncel",
		"link": "https://www.aa.com.tr/tr"
	},
	"cnnturk": {
		"rss": "https://www.cnnturk.com/feed/rss/all/news",
		"link": "https://www.cnnturk.com/"
	}
}
```

- Oluşturulan json dosyasındaki haberler düzenlenmek üzere Zemberek işlemine sokuldu
- Zemberek ile düzenlenen metinler sınıflandırılarak aynı haberler tespit edildi
- Bulunan benzer haber metinlerindeki haberler özetlendi
- Çalışma web ve mobil arayüzünde sunuldu


## Faydalanılan Kaynaklar
### Ortam ve Kütüphaneler
-VSCode, Android Studio
-Ubuntu Linux, Windows, MacOS
-Python 3.8
-JPype1 0.7.0
-feedparser
-newspaper


## Kurulumlar

## Derleme ve Çalıştırma


###  Referanslar
* [http://zembereknlp.blogspot.com/](http://zembereknlp.blogspot.com/)
* [https://www.aclweb.org/anthology/W17-1003/](https://www.aclweb.org/anthology/W17-1003/)

### Repository
* [https://github.com/ozturkberkay/Zemberek-Python-Examples](https://github.com/ozturkberkay/Zemberek-Python-Examples)
*  [https://github.com/gaetangate/text-summarizer/tree/master/text_summarizer](https://github.com/gaetangate/text-summarizer/tree/master/text_summarizer)
*  [https://holwech.github.io/blog/Automatic-news-scraper/](https://holwech.github.io/blog/Automatic-news-scraper/)
[https://github.com/holwech/NewsScraper](https://github.com/holwech/NewsScraper)


## Lisans
Bu proje **GPL v3** lisansı ile lisanslanmış olup, lisans detaylarını [LICENSE](https://github.com/fourplusone41/TezHaber/blob/master/LICENSE) sayfasına bakabilirsiniz.
