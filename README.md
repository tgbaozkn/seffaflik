# Enerji Piyasaları İşletme A.Ş. (EPİAŞ)
[EPİAŞ](https://www.epias.com.tr/)’ın başlıca amacı ve faaliyet konusu,
“ Piyasa işletim lisansında yer alan enerji piyasalarının etkin, şeffaf,
güvenilir ve enerji piyasasının ihtiyaçlarını karşılayacak şekilde planlanması,
kurulması, geliştirilmesi ve işletilmesidir. Eşit taraflar arasında ayrım
gözetmeden güvenilir referans fiyat oluşumunun temin edilmesi ve artan piyasa
katılımcı sayısı, ürün çeşitliliği ve işlem hacmiyle likiditenin en üst düzeye
ulaştığı, piyasa birleşmeleri yoluyla ticaret yapılmasına imkan tanıyan bir
enerji piyasası işletmecisi olmaktır.”

# EPİAŞ Şeffaflık Platformu
EPİAŞ, işlettiği piyasalarda katılımcıların işlemlerini fırsat eşitliliği
çerçevesinde yürütebilmesi, piyasadaki bilgi asimetrisinin önlenmesi ve
katılımcıların yapacakları işlemlerde doğru karar verebilmeleri için bir merkezi
veri ve analiz platformu olan [“Şeffaflık Platformunu”](https://seffaflik.epias.com.tr) işletmektedir.

EPİAŞ Şeffaflık Platformundaki hizmet kalitesini artırmak maksadıyla ayrıca
kullanıcılarına “Web Servis Hizmeti” de sunmaktadır. Talep eden kullanıcılar
platformda yayımlanan tüm verilere buradan da kolaylıkla ulaşabilmektedir.
Şeffaflık Platformu Web Servis Hizmetini ve dolayısıyla bu kütüphaneyi
kullanacak kişilerin öncelikle belirtmiş oldukları IP numarası üzerinden Şeffaflık Platformu Web Servis
Hizmeti ile tüm verilere ulaşabilme iznini almaları geremektedir. Bunun için
öncelikle kullanıcıların Şeffaflık Platformunda yayımlanan
[Web Servis Şartnamesini](https://www.epias.com.tr/wp-content/uploads/2016/10/Web-Servis-%C5%9Eartnamesi-1.docx)
doldurmaları ve "seffaflik@epias.com.tr" mail adresi üzerinden doldurulmuş
şartnameyi firma ile paylaşmaları gerekmektedir.

## Kurulum
### Gereksinimler (Requirements)
seffaflik kütüphanesinin kullanımı için gerekli paketler:
* pandas
* requests
* python-dateutils
### pip aracılığıyla en son sürümü yükleyin
```
$ pip install seffaflik
```

### Kimlik (Client Id) Oluşturulması
```python
import seffaflik
seffaflik.ortak.anahtar.kimlik_dosyasi_olustur(istemci_kimligi="abcdefg")
```
Yukarıdaki işlemi gerçekleştirmenizden sonra ana dizininize özel bir
.seffaflik/.kimlik dosyası yerleştirir. ~/.seffaflik/.kimlik dosyanız aşağıdaki
gibi görünmelidir:
```python
{
  "istemci_kimligi": "abcdefg"
}
```

