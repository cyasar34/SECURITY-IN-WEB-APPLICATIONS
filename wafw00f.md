## Wafw00f
<p align="justify">Kali Linux dahilinde bulunan ve web uygulama güvenlik duvarlarını (WAF) tespit etmek için kullanılan bir
araçtır. Bir hedef siteye çeşitli HTTP istekleri göndererek hangi WAF türünün kullanıldığını belirler. </p>

### Wafw00f Nasıl Çalışır?
<li>Web sitesine özel HTTP istekleri gönderir ve yanıtları analiz ederek WAF'ın varlığını ve türünü tespit eder.</li>
<li>Eğer bir site WAF kullanıyorsa, belirli HTTP yanıt kodları, başlıklar veya hata mesajları verir.</li>
<li>Wafw00f, bu yanıtları bilinen WAF imzalarıyla karşılaştırarak sonucu belirler.</li>

### Wafw00f Türleri:
<li>Bulut Tabanlı WAF'lar (Cloud-Based WAFs): Bu tür WAF'lar, genellikle CDN hizmetleri ile entegre çalışır ve trafiği bir ara sunucudan geçirerek güvenlik sağlar.</li>
<li>Donanım Tabanlı (Appliance) WAF'lar: Bu tür WAF'lar, fiziksel veya sanal makineler üzerinde çalışarak güvenlik sağlar. </li>
<li>Açık Kaynaklı WAF'lar: Bu tür WAF'lar, genellikle ücretsizdir ve geliştiriciler tarafından özelleştirilebilir.</li>
<li>Şirket İçin Özel WAF'lar: Bazı büyük şirketler, kendi ihtiyaçlarına göre özelleştirilmiş WAF çözümleri geliştirir.</li>

### En yaygın kullanılan theHarvester parametreleri
| PARAMETRE | AÇIKLAMA | 
| :---         |     :---:      |       
| -v | Komut satırı uygulamalarında "verbose" modunu etkinleştirir. Verbose modu, uygulamanın daha fazla çıktı üretmesini, yani daha detaylı bilgi vermesini sağlar. |
| -a | Eğer birden fazla WAF kullanılıyorsa, hepsini tespit etmeye çalışır. |
| -r | "no redirect" veya "yönlendirmeyi takip etme" seçeneğini ifade eder. Bu parametre kullanıldığında, araç 3xx HTTP durum kodları ile yapılan yönlendirmeleri takip etmeyecektir. Yani, eğer hedef web sitesi bir isteğe 3xx durum kodu ile yanıt verirse ve bu yanıt bir başka URL'ye yönlendirme içeriyorsa, bu yönlendirmeyi takip etmez ve sadece orijinal URL için cevapları analiz eder. |
| -h | Yardım mesajını görüntüler. |
| -t | Sadece belirli bir WAF’ı test etmek için kullanılır. |
| -o | Çıktıyı belirli bir dosyaya kaydeder. |
| -i | Hedefleri bir dosyadan okumak için kullanılır. |
| -l | Bu aracın tespit edebileceği tüm Web Uygulama Güvenlik Duvarı (WAF) türlerini listelemek için kullanılır. |

#### wafw00f Ekran Görüntüsü
![wafw00f](https://github.com/cyasar34/SECURITY-IN-WEB-APPLICATIONS/blob/main/wafw00f.PNG)

### Örnek Kullanım Senaryoları
<p align="justify"><li>•	Sistemde bulunan tüm Web Uygulama Güvenlik Duvarı (WAF) listesini bulmayı sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> wafw00f –l <br><br>




> **Yasal Sınırlar:** wafw00f gibi araçlar yalnızca yasal ve yetkili testlerde kullanılmalıdır. İzinsiz kullanım yasa dışıdır. <br>





 
