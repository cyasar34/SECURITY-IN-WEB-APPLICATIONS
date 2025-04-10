## Http Durum Kodları (HTTP Status Codes)

#### 1XX (100 Kodlu Yanıtlar):
<li>Kullanıcının bulunduğu isteğin sunucu tarafında devam ettiğinin bildirildiği yanıtlardır.
Örneğin HTTP 100 yanıtı isteğin şu anda işlenmekte olduğunun bildirildiği yanıttır. Bu yanıt tarayıcıya iletilir ancak
kullanıcı ekranına yansıtılmaz. <b>Kısacası bilgi isteği.</b></li>
<b>100 Continue:</b> İstemci, isteğin geri kalanını göndermeye devam edebilir.<br>
<b>101 Switching Protocols:</b> Sunucu, istemcinin istediği protokol değişikliğini kabul eder (örneğin, HTTP'den WebSocket'e
geçiş).<br>
<b>102 Processing:</b> Sunucu, isteği işliyor ancak henüz yanıt hazır değil.<br><br>

#### 2xx (200 Kodlu Yanıtlar): 
<li>Tarayıcıdan sayfaya yönelik sunucuya gönderilen işlemin başarılı olduğunun bildirildiği
yanıtlardır. HTTP 2xx kodlu yanıtlarda sunucunun tarayıcıdan gelen isteğe başarılı yanıt verdiği ve sayfanın açılabilir
olduğu bildirilir. <b>Kısacası başarı.</b></li>
<b>200 OK:</b> İstek başarılı oldu ve yanıt gönderildi.<br>
<b>201 Created:</b> Yeni bir kaynak başarıyla oluşturuldu (genellikle POST isteklerinde kullanılır).<br>
<b>202 Accepted:</b> İstek kabul edildi ancak henüz işlenmedi.<br>
<b>204 No Content:</b> İstek başarılı oldu ancak yanıt gövdesi yok (örneğin, DELETE isteklerinde).<br>
<b>206 Partial Content:</b> İstemci, kaynağın sadece bir kısmını istediğinde kullanılır (örneğin, dosya indirme).<br>

#### 3xx (300 Kodlu Yanıtlar): 
<li>Tarayıcıdan web sayfasına yönelik sunucuya iletilen isteğin farklı bir sayfaya yönlendirildiğinin
bildirildiği yanıtlardır. <b>Kısacası yönlendirme.</b></li>
<b>301 Moved Permanently:</b> Kaynak kalıcı olarak başka bir URL'ye taşındı.<br>
<b>302 Found:</b> Kaynak geçici olarak başka bir URL'de bulunuyor.<br>
<b>304 Not Modified:</b> Kaynak değişmediği için istemci önbelleğini kullanabilir (Cache-Control ile birlikte kullanılır).<br>

#### 4xx (400 Kodlu Yanıtlar): 
<li>Kullanıcı kaynaklı bir hatanın gerçekleştiğinin bildirildiği yanıtlardır. Yani HTTP 4xx hata kodlu
bir yanıt tarayıcıya gönderildiğinde burada hatanın kaynağının client yani kullanıcı olduğu bildirilir. Ancak burada ki
kullanıcı salt tarayıcıdan isteği gönderen kişi olarak algılanmamalıdır. Web sayfasını barındıran sitede uygulanan
herhangi bir işlem sonrasında 4xx HTTP hata kodları ortaya çıkabilir. <b>Kısacası istemci hatası.</b></li>
<b>400 Bad Request:</b> İstek geçersiz veya hatalı formatta.<br>
<b>401 Unauthorized:</b> İstek için kimlik doğrulama gerekiyor.<br>
<b>403 Forbidden:</b> İstemcinin kaynağa erişim izni yok.<br>
<b>404 Not Found:</b> İstenen kaynak bulunamadı.<br>
<b>405 Method Not Allowed:</b> İstenen HTTP metodu bu kaynak için desteklenmiyor.<br>
<b>408 Request Timeout:</b> İstek zaman aşımına uğradı.<br>
<b>429 Too Many Requests:</b> İstemci çok fazla istek gönderdi (rate limiting).<br>

#### 5xx (500 Kodlu Yanıtlar): 
<li>Tarayıcıdan gönderilen istek sırasında sunucu kaynaklı bir hatanın ortaya çıktığının iletildiği
yanıtlardır. <b>Kısacası sunucu hatası.</b></li>
<b>500 Internal Server Error:</b> Sunucu beklenmeyen bir hata ile karşılaştı.<br>
<b>501 Not Implemented:</b> Sunucu, istenen metodu desteklemiyor.<br>
<b>502 Bad Gateway:</b> Sunucu, bir ağ geçidi veya proxy olarak çalışırken geçersiz bir yanıt aldı.<br>
<b>503 Service Unavailable:</b> Sunucu geçici olarak hizmet veremiyor (bakım veya aşırı yük nedeniyle).<br>
<b>504 Gateway Timeout:</b> Sunucu, bir ağ geçidi veya proxy olarak çalışırken zaman aşımına uğradı.<br>
<b>505 HTTP Version Not Supported:</b> Sunucu, istekte kullanılan HTTP sürümünü desteklemiyor.<br>






 
