## Nmap
<p align="justify">Nmap aracı port taramalarında en stabil ve en çok kullanılan bir araçtır. Sadece port tarama değil işletim sistemi tespiti,
ağ haritalama, ağ tarama işlemlerinde kullanılabilir. Açık kaynak kodlu ve ücretsizdir. Nmap aracı Kali Linux ile birlikte
gelmektedir. Aynı zamanda Windows, Mac ve Unix sistemlerinin hepsinde kullanmak mümkündür.</p>
  
### Nmap Temel Özellikleri:
<li>Ağ Keşfi (Host Discovery): Bir ağdaki aktif cihazları (host'ları) tespit eder. Örneğin, bir IP aralığındaki tüm cihazları bulur. </li>
<li>Port Tarama (Port Scanning):  Hedef cihazdaki açık portları ve bu portlarda çalışan hizmetleri tespit eder. Örneğin, bir sunucuda hangi portların açık olduğunu ve hangi hizmetlerin çalıştığını gösterir. </li>
<li>İşletim Sistemi Tespiti (OS Fingerprinting): Hedef cihazın işletim sistemini tahmin eder. Örneğin, bir cihazın Linux mu yoksa Windows mu çalıştırdığını belirler. </li>
<li>Hizmet ve Sürüm Tespiti (Service/Version Detection): Portlarda çalışan hizmetlerin türünü ve sürümünü belirler. Örneğin, bir web sunucusunun Apache mi yoksa Nginx mi çalıştırdığını ve sürüm numarasını gösterir.</li>
<li>Script Taraması (NSE - Nmap Scripting Engine):Nmap Scripting Engine (NSE) ile özelleştirilmiş taramalar yapar. Örneğin, güvenlik açıklarını tespit etmek veya belirli hizmetler hakkında bilgi toplamak için kullanılır. </li>
<li>Ağ Haritalama (Network Mapping):Bir ağın topolojisini çıkarır ve cihazlar arasındaki bağlantıları gösterir.</li>

### Nmap scriptleri (NSE - Nmap Scripting Engine)
<p align="justify">Nmap'in yeteneklerini genişleten ve otomatik olarak çeşitli görevleri
gerçekleştiren betiklerdir. Bu betikler, ağ taraması, servis tespiti, güvenlik açığı taraması ve daha birçok işlevi
otomatikleştirmek için kullanılır. Bu betikler, Lua programlama dili ile yazılır ve aşağıdaki gibi çeşitli amaçlar için
kullanılabilir:</p>
<li>Servis ve sürüm tespiti</li>
<li>Güvenlik açığı taraması</li>
<li>Ağ keşfi</li>
<li>Veri toplama</li>
<li>Otomatik exploit denemeleri</li>
Nmap, birçok önceden tanımlanmış betikle birlikte gelir. Bu betikler, /usr/share/nmap/scripts dizininde (Linux
sistemlerde) bulunur.
Nmap betikleri, belirli kategorilere ayrılmıştır. Bazı önemli kategoriler şunlardır:
<li><b>auth:</b> Kimlik doğrulama ile ilgili betikler.</li>
<li><b>default:</b> Varsayılan taramalarda kullanılan betikler.</li>
<li><b>discovery:</b> Ağ keşfi yapan betikler.</li>
<li><b>exploit:</b> Güvenlik açıklarını tespit etmeye yönelik betikler.</li>
<li><b>vuln:</b> Güvenlik açıklarını tarayan betikler.</li>
<li><b>safe:</b> Sistemlere zarar vermeyen güvenli betikler.</li>


### En yaygın kullanılan Nmap parametreleri

| PARAMETRE | AÇIKLAMA | 
| :---         |     :---:      |       
| # nmap 192.168.1.1 | Tek bir ip için gerçekleştirilen testi ifade eder. |
| # nmap www.testphp.vulnweb.com | Domaine gerçekleştirilen testi ifade eder. |
| # nmap –iL iplistesi.txt | Doküman içerisinde bulunan adreslere yapılacak testi ifade eder.|
| # nmap 192.168.1.1 -10  | 1-10 ipleri dahil olmak üzere arasında gerçekleştirilen testi ifade eder. |
| # nmap –sP 192.168.1.1 / 24 | Tüm sistemlere ping atarak, yanıt veren sistemlerin açık ya da kapalı olduğunu tespit eder. (Ping Sweep) |
| # nmap –PS 192.168.1.1 /24 | TCP SYN ping paketleri ile sistemlerin açık ya da kapalı olduğunu tespit eder. (Ping SYN) |
| # nmap –PA 192.168.1.1 /24 | TCP ACK ping paketleri ile sistemlerin açık ya da kapalı olduğunu tespit eder. (Ping ACK) |
| # nmap –PU 192.168.1.1 /24 | UDP ping paketleri ile sistemlerin açık ya da kapalı olduğunu tespit eder. (Ping UDP) |
| # nmap –sS 192.168.1.1 | Hedefe TCP Syn paketi gönderir. Portlar açık ise SYN-ACK yanıt dönecektir. Tarama yapan makine ise RST paketi göndererek tarama sonlandırılacaktır. Burada üçlü el sıkışması tamamlanmadan işlem biter. (TCP Syn Scan) |
| # nmap –sT 192.168.1.1 | Bu tarama ‘TCP Syn Scan’ ile benzerlik gösterir. Bu benzerlik portların kapalı olduğu durumlardaki hedefin göndereceği RST-ACK paketleridir. Burada üçlü el sıkışması tamamlanır ve sistem sonrasında loglanır. (TCP Connect Scan) |
| # nmap –sU 192.168.1.1 | Udp portlarının genel durumunu analiz etmek için kullanılır. (UDP Scan) |
| # nmap –sA 192.168.1.1 | Güvenlik duvarının konfigürasyon durumunu durumunu analiz etmek için kullanılır. (ACK Scan) |
| # nmap –sW 192.168.1.1 | Bu tarama şeklinde dönen yanıtların RST frame boyutlarına göre açık ya da kapalı olduğunu öğrenebiliriz. (Windows Scan) |
| # nmap –O 192.168.1.1 | İşletim sistemini tespit etmemizi sağlar. (OS Analizi) |
| # nmap –oN deneme.txt 192.168.1.1 | Tarama çıktısını istenilen formatta verir. |
| # nmap –oX deneme.xml 192.168.1.1 | XML formatında çıktı verir. |


### Nmap Ekran Görüntüsü
![Nmap](https://github.com/cyasar34/SECURITY-IN-WEB-APPLICATIONS/blob/main/nmap.PNG)

### Örnek Kullanım Senaryoları

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresli hedefe TCP Syn Scan paketi göndermeyi sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –sS –v 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak www.google.com.tr adresinde bulunan UDP portlarından en sık kullanılan 10 portunu udplistesi.xml dokümanına kaydetmeyi sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –sU –top-ports 10 –oX udplistesi.xml www.google.com.tr

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresindeki açık portlarda çalışan hizmetlerin sürüm bilgilerini sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –sV –v 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresindeki HTTP hizmetiyle ilgili bilgi toplamak için kullanılan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –script=http-title 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak www.gelisim.edu.tr adresinin işletim sistemini tespit etmeyi ve bulunan sonuçları ‘gelisim.txt’ dokümanına kaydetmeyi sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –O www.gelisim.edu.tr –oN gelisim.txt

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresine TCP ACK ping paketi göndermeyi ve güvenlik duvarının durumunu görüntülemeyi sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –PA –sA 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak scanme.nmap.org adresinde http-title ve http-headers scriptlerini çalıştırmayı sağlayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –script=http-title,http-headers scanme.nmap.org

<p align="justify"><li>Nmap tool’u kullanarak scanme.nmap.org sistemdeki bilinen güvenlik açıklarını tarayan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –script=vuln scanme.nmap.org

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresindeki bilinen güvenlik açıklarını tespit etmek için kullanılan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –script=vuln 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresine yapılan tarama sonuçlarını ‘output.txt’ dosyasına kaydetmek için kullanılan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –oN output.txt 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.1 ip adresindeki FTP hizmetiyle ilgili bilgi toplamak için kullanılan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –script=ftp-anon 192.168.1.1

<p align="justify"><li>Nmap tool’u kullanarak 192.168.1.0/24 ağındaki cihazların bağlantılarını ve topolojisini çıkarmak için kullanılan komut bloğunu yazınız?</li></p>
<b>Komut:</b> nmap –sn –traceroute 192.168.1.0/24 <br><br><br>


> **Yasal Sınırlar:** Nmap gibi araçlar yalnızca yasal ve yetkili testlerde kullanılmalıdır. İzinsiz kullanım yasa dışıdır. <br>





 
