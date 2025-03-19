## Dmitry
<p align="justify">Kali Linux üzerinde bulunan dmitry, sızma testlerinde sıklıkla kullanılan bir pasif bilgi toplama aracıdır. Bu araç, bir hedef hakkında çeşitli bilgileri toplamak için kullanılır ve özellikle IP adresleri, domain bilgileri, port taramaları ve daha fazlasını keşfetmeye yardımcı olur.
Dmitry, açık kaynaklı bir araçtır ve özellikle hızlı ve basit bilgi toplama ihtiyaçları için idealdir. </p>

### Dmitry'nin Temel Özellikleri:
<li>Whois Sorguları: Hedef domain veya IP adresi hakkında whois bilgilerini toplar. Domain kayıt bilgileri, sahibi, kayıt tarihi ve son kullanma tarihi gibi detayları içerir.</li>
<li>Netcraft Veri Toplama: Hedef domainle ilgili Netcraft üzerinden bilgi toplar.</li>
<li>Alt Alan Adı (Subdomain) Keşfi: Hedef domainin alt alan adlarını tespit eder.</li>
<li>Port Tarama: Hedef IP adresinde açık portları tarar. Temel port tarama özelliği sunar (Nmap gibi detaylı değildir).</li>
<li>E-posta Adresi Toplama: Hedef domainle ilişkili e-posta adreslerini toplar. </li>

### En yaygın kullanılan dmitry parametreleri
| PARAMETRE | AÇIKLAMA | 
| :---         |     :---:      |       
| -o | Elde edilen bilgilerin kaydedileceği dosya yolunu belirtebilirsiniz. |
| -i | Ip adresi üzerinden who is sorgulaması sağlayabilirsiniz. |
| -w | Domain üzerinden who is sorgulaması gerçekleştirebilirsiniz.|
| -n | Sorgulanan sitenin, netcraft.com’da yer alan bilgilerini denetleyebilirsiniz. |
| -s | Sitenin mevcut sub domainlerini tespit edebilirsiniz. |
| -e | Mail adreslerini bulabilirsiniz. |
| -f | Filtrelenmiş TCP Portlarını bulabilirsiniz. |
| -p | Genel port tarama işlemi sağlayabilirsiniz. |

#### dmitry Ekran Görüntüsü
![theHarvester](https://github.com/cyasar34/SECURITY-IN-WEB-APPLICATIONS/blob/main/dmitry.PNG)

### Örnek Kullanım Senaryoları
<p align="justify"><li>Dmitry tool’u kullanarak gelisim.edu.tr üzerinde subdomainleri ve mail adreslerini bulup “test2” dokümanına kaydeden komut bloğunu yazınız?</li></p>
<b>Komut:</b> dmitry –w gelisim.edu.tr –se –o test2

<p align="justify"><li>Dmitry tool’u kullanarak gelisim.edu.tr ip adresini ve netcraft üzerinde tarama yapıp bulunan verileri “test3” dokümanına kaydeden komut bloğunu yazınız?</li></p>
<b>Komut:</b> dmitry –in gelisim.edu.tr –o test3 <br><br>

> **Yasal Sınırlar:** dmitry gibi araçlar yalnızca yasal ve yetkili testlerde kullanılmalıdır. İzinsiz kullanım yasa dışıdır. <br>









 
