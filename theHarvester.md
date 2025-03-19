## theHarvester
Kali Linux üzerinde bulunan theHarvester, sızma testlerinde sıklıkla kullanılan bir pasif bilgi toplama aracıdır. Pasif bilgi toplama, hedef sistemlerle doğrudan etkileşime girmeden bilgi elde etme anlamına gelir.
theHarvester, çeşitli açık kaynaklardan bilgi toplamak için kullanılır. Bu araç, bir hedef hakkında geniş kapsamlı bilgi toplamak için kullanılır ve özellikle e-posta adresleri, alt alan adları (subdomains), ana bilgisayar adları (hostnames) ve IP adresleri gibi bilgileri keşfetmeye yardımcı olur. 

### theHarvester'ın Temel Özellikleri:
<li>E-posta Adresi Toplama: Hedef domain ile ilişkili e-posta adreslerini toplar.</li>
<li>Alt Alan Adı (Subdomain) Keşfi: Hedef domainin alt alan adlarını tespit eder.</li>
<li>Ana Bilgisayar (Host) ve IP Adresi Keşfi: Hedef domainle ilişkili sunucuların IP adreslerini ve ana bilgisayar adlarını listeler.</li>
<li>Çeşitli Veri Kaynakları: Google, Bing, LinkedIn, Twitter, Shodan, VirusTotal gibi farklı kaynaklardan veri toplar.</li>
<li>Esnek Kullanım:Komut satırı arayüzü (CLI) üzerinden kullanılır.</li>

### En yaygın kullanılan theHarvester parametreleri
| PARAMETRE | AÇIKLAMA | 
| :---         |     :---:      |       
| -d | Taranacak hedef alan adını veya IP adresini belirtir. |
| -b | Kullanılacak kaynakları belirtir. Birden fazla kaynak seçmek için virgülle ayırınız. |
| -f | Çıktı formatını belirtir. XML ve JSON formatında çıktı verir.|
| -h | Yardım mesajını görüntüler. |
| -v | Verbose modu etkinleştirir. Bu mod, daha fazla bilgi içeren çıktılar üretir. |
| -l | Limit değerini belirtir. |
| -s | Sorgulanan alan adının Shodan üzerinden bilgi toplanır. |
| -c | Brute force yöntemi ile subdomainleri bulmayı sağlar. |












 
