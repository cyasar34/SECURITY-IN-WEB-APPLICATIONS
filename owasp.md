## OWASP (Open Web Application Security Project) Nedir?
<p align="justify">OWASP (Open Web Application Security Project), web uygulama güvenliği alanında çalışan, kar amacı gütmeyen
bir kuruluştur. OWASP, geliştiricilere, güvenlik uzmanlarına ve kuruluşlara ücretsiz kaynaklar, araçlar ve rehberler
sunarak güvenli yazılım geliştirme ve güvenlik açıklarını önleme konusunda destek sağlar.

### Owasp Top 10

<p align="justify">OWASP Top 10, web uygulama güvenliği alanında en yaygın ve kritik güvenlik açıklarını listeleyen, dünya çapında kabul görmüş bir rehberdir.
Bu liste, uygulama geliştiriciler, güvenlik uzmanları ve şirketler için hem farkındalık oluşturmak hem de güvenlik önlemleri geliştirmekte bir başlangıç noktası sağlamak amacıyla kullanılır.</p>
  
![Owasp Top Ten](https://github.com/cyasar34/SECURITY-IN-WEB-APPLICATIONS/blob/main/owasp_top_ten.png)


| Owasp Top 10 | Tanımı |
| :---         |     :---:      |
| A01:2021 - Broken Access Control (Bozuk Erişim Kontrolü)  |  Kısacası, yetkisiz kullanıcıların hassas kaynaklara erişmesine izin verir.     |
| A02:2021 - Cryptographic Failures (Şifreleme Hataları) |	Kısacası, hassas verilerin şifrelenmemesi veya zayıf şifreleme algoritmalarının kullanılması. |
| A03:2021 - Injection (Enjeksiyon) |	Kısacası enjeksiyonu saldırıları, saldırganlar tarafından veritabanındaki gizli bilgilere erişmek için kullanılmaktadır. Web uygulamalarının giriş alanlarına kötü amaçlı karakterler girilerek, SQL sorgusunun değiştirilmesi ile gerçekleştirilmektedir. |
| A04:2021 - Insecure Design (Güvensiz Tasarım) |	Kısacası, güvenlik gereksinimlerinin tasarım aşamasında dikkate alınmaması. |
| A05:2021 - Security Misconfiguration(Yanlış Güvenlik Yapılandırması) |	Kısacası, yanlış güvenlik yapılandırmaları, güvenlik ayarlarının düzgün bir şekilde tanımlanmadığı ve uygulanmadığı, varsayılan değerlerin korunmadığı durumlarda ortaya çıkmakta ve güvenlikle ilgili ciddi sorunlara neden olmaktadır. |
| A06:2021 - Vulnerable and Outdated Components(Savunmasız ve Eski Bileşenler)	| Kısacası OWASP’a göre bir sistemi oluşturan bileşenlerinin tamamının sürümleri bilinmediğinde, yazılımların desteklenmediği veya güncel olmadığı durumlarda, güvenlik açıkları düzenli olarak taranmadığında, yazılım geliştiricileri tarafından güncellenen, yükseltilen veya yama olarak uygulanan kütüphanelerin uyumluluğu test edilmediği durumlarda o sistem savunmasız halde olmaktadır. |
| A07:2021 - Identification and Authentication Failures (Tanımlama ve Kimlik Doğrulama Hataları) |	Kısacası, tanımlama ve kimlik doğrulama hataları, bir saldırganın sistemdeki herhangi bir hesabın kontrolünü ele geçirmek için manuel veya otomatik yöntemler kullanmasına veya daha kötüsü sistem üzerinde tam kontrol sağlamasına izin verebilir. |
| A08:2021 - Software and Data Integrity Failures (Yazılım ve Veri Bütünlüğü Hataları) |	Kısacası, yazılım ve veri bütünlüğü arızaları, bütünlük saldırılarına karşı korumasız kodlar ve altyapı ile ilgilidir. |
| A09:2021 - Security Logging and Monitoring Failures (Güvenlik Günlüğü ve İzleme Hataları) | Kısaca, saldırıların tespit edilmemesi veya geç tespit edilmesi. |
| A10:2021 - Server-Side Request Forgery (SSRF - Sunucu Tarafı İstek Sahteciliği) | Kısaca, sunucunun harici kaynaklara istek göndermesine neden olan açıklar. |

### OWASP'ın web uygulamalarındaki güvenlik açıklarını taramaya yardımcı olmak için hazırladığı aracın adı nedir?
<p align="justify">OWASP ZAP, Kali ile gelen ve web zafiyetlerini otomatik olarak tespit eden açık kaynak kodlu bir web güvenlik
tarayıcısıdır. Proxy sunucu olarak kullanılabilir ve bu sayede https trafiği de dahil olmak üzere aracın içinden geçen tüm
trafik değiştirilebilir.</p> <br><br>

> **Yasal Sınırlar:** Owasp ZAP gibi araçlar yalnızca yasal ve yetkili testlerde kullanılmalıdır. İzinsiz kullanım yasa dışıdır. <br>



