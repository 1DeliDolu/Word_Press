# WordPress Glossary

## 📖 WordPress Sözlüğü (WordPress Glossary)

Bu belge, WordPress’e özgü çeşitli terimlerin tanımlarını sunmak amacıyla hazırlanmıştır. Kullanıcıların aşina olmayabileceği kavramları açıklar.

Eğer bir katkıcıysanız, lütfen genel terimlerin (API, PHP, JavaScript vb.) tanımlarını eklemeyiniz.

---

## 📂 Mutlak Yol (Absolute Path)

(bir diğer adıyla tam yol – full path)

Bir dosyanın veya dizinin bilgisayar dosya sistemi içerisindeki tam konumudur. Bir mutlak yol, kök dizinden (veya sürücü harfinden) başlar ve hiyerarşi boyunca belirli dosya veya dizine ulaşana kadar devam eder. Bu, kök dizinden başlamayan göreli yol (relative path) ile zıttır.

Mutlak yolların yazım biçimi işletim sistemine göre değişir. Microsoft Windows’ta bir sürücü harfi ile başlar ve dizin adlarını ayırmak için ters eğik çizgi (`\`) kullanır. macOS ve Linux’ta sürücü harfi yoktur ve dizin ayırıcısı olarak düz eğik çizgi (`/`) kullanılır.

Örnekler:

* Windows: `C:\Users\Matt\www\blog\images\icecream.jpg`
* macOS: `/Users/Matt/www/blog/images/icecream.jpg`
* Linux: `/home/Matt/www/blog/images/icecream.jpg`

Bir web sayfasını barındıran dizinin mutlak dosya sistem yolunu bulmak için aşağıdaki kodu yeni bir metin dosyasına kopyalayın, dosyayı `path.php` olarak kaydedin (basit bir PHP web sayfası) ve sunucunuza yükleyin. Ardından tarayıcınızda o dosyanın URL’sine gidin (örn. `http://www.example.com/path.php`).

```php
<?php
echo getcwd();
?>
```

Bkz.: Path (computing) – Wikipedia

---

## 🌐 Mutlak URI (Absolute URI)

(bir diğer adıyla tam URI – full URI)

Bir kaynağın tam konumunu içeren URI’dir. (Göreli URI ile karşıtlık oluşturur.)

Örnekler:

* `http://www.example.com/blog/images/icecream.jpg`
* `ftp://ftp.example.com/users/h/harriet/www/`

---

## ⚡ Eylem (Action)

WordPress içinde; bir **Action**, WordPress Çekirdeği (WordPress Core) boyunca belirli noktalarda çalıştırılan bir PHP fonksiyonudur.

Geliştiriciler, mevcut herhangi bir Hook belirterek Action API’sini kullanarak özel bir Action oluşturabilir, mevcut bir Action’dan kod ekleyip kaldırabilir. Bu işleme “hooking” denir.

Örnek: Bir geliştirici, bir Tema’nın altbilgisine (footer) kod eklemek isteyebilir. Bu, yeni bir fonksiyon yazarak ve onu `wp_footer` Action’una “hook” ederek yapılabilir.

Özel Actions, özel Filters’tan farklıdır. Çünkü özel Actions mevcut Action’lara kod eklemenize veya çıkarmanıza izin verir. Özel Filters ise mevcut bir Action içindeki belirli bir veriyi (örneğin bir değişken) değiştirmenizi sağlar.

Bkz.: Filter, Hook, Terminology Confusion
İlgili makaleler: Actions, Action Reference, `add_action()`
Forum gönderileri: Filters vs. Actions Discussion and Explanation

---

## 🛠️ Yönetici Çubuğu (Admin Bar)

Sitenizin hemen üzerinde bulunan ve yeni bir yazı eklemek veya profilinizi düzenlemek gibi özelliklere hızlı erişim sağlayan ekran alanıdır. Yalnızca oturum açtığınızda görünür.

Yönetici çubuğu, WordPress 3.1 sürümünde eklenmiş, WordPress 3.3 sürümünde ise Araç Çubuğu (Toolbar) ile değiştirilmiştir. Açmak (veya kapatmak) için: **Gösterge Paneli (Dashboard) > Yönetim (Administration) > Kullanıcılar (Users) > Profiliniz (Your Profile)** yolunu izleyin.

İlgili makaleler: Toolbar
Bkz.: Your Profile Screen

---

## 🔄 Ajax

Ajax, web sayfalarının sunucuda belirli işlemleri sayfa yeniden yüklenmeden gerçekleştirmesini sağlayan bir tekniktir.

Örnek: Bir WordPress blogunda bir yorumu onayladığınızda, WordPress bu işlemi Ajax ile gerçekleştirir ve sayfayı yeniden yüklemeden yorumun durum değişikliğini görürsünüz.

İlgili makale: AJAX
Dış bağlantı: AJAX – Wikipedia

---

## 🌍 Apache

Apache, **Apache HTTP Server Project**’in kısaltmasıdır. Güçlü, ticari kaliteye sahip, özellikli ve özgürce erişilebilen açık kaynak HTTP web sunucusu yazılımıdır. **Apache Software Foundation** tarafından üretilir.

İnternette en yaygın kullanılan web sunucusudur ve Windows, Unix/Linux ve Mac OS X dâhil birçok platformda çalışır. WordPress tabanlı siteler yayınlamak için güçlü bir temel sunar.

---

## 🔌 API

Tanım için lütfen Wikipedia sayfasına bakınız.

---

## 📊 Dizi (Array)

Bir **array (dizi)**, bilgisayar programlamasında kullanılan temel veri yapılarından biridir. Sayısal veya metinsel değerlerden oluşan bir listedir. Diziler, programcılara verilere rastgele erişim sağlar. Tek boyutlu veya çok boyutlu dizilerde veri saklanabilir.

Örnek bir boyutlu dizi (7 elemanlı):

```
105  200  54  53  102  13  405
```

`wp_list_categories()` şablon etiketi (`Template Tag`), `exclude` parametresi için tek boyutlu bir dizi kullanır.

Örnek iki boyutlu dizi (7x3):

```
105  200  54  53  102  13   405
15   210  14  513  2    2313 4512
501  500  499 488  552  75   1952
```

Dış bağlantılar: Array Programming – Wikipedia, Array – freedictionary.com

---

## 🔡 ASCII

**ASCII** (okunuşu: “ask ee”), yalnızca İngilizce harfler, sayılar, birkaç yaygın sembol ve noktalama işaretleri içeren standart ama sınırlı bir karakter kümesidir. WordPress içeriği ASCII ile sınırlı değildir; herhangi bir Unicode karakteri de içerebilir.

ASCII, **American Standard Code for Information Interchange**’ın kısaltmasıdır.

Dış bağlantılar: ASCII – Wikipedia (karakter tablosu ile birlikte)

---

## 📰 Atom

Haber benzeri sitelerde içeriği dağıtmak için kullanılan bir biçimdir. Atom uyumlu programlar (haber okuyucular veya toplayıcılar – aggregators) tarafından görüntülenebilir.

Bkz.: News reader, RSS, RDF
Dış bağlantılar: Atom (standard) – Wikipedia

## 🧩 Öznitelik Kaynakları (Attribute sources)

Bir bloğun öznitelik yapısını tanımlayan nesnedir. Anahtarlar, bir blok türünün durumunu tanımlamak için en uygun şekilde adlandırılabilir. Her anahtarın değeri, öznitelik değerinin kaydedilmiş bir yazının içeriğinden nasıl çıkarılacağını tanımlayan bir işlevdir. İşlendiğinde, öznitelik kaynaklarında tanımlanan anahtarların biçiminde yeni bir nesne oluşturulur; her değer, öznitelik kaynağı işlevinin sonucudur.

---

## 📝 Öznitelikler (Attributes)

Bir bloğun yazı içeriğindeki mevcut durumunun nesne temsili. Kaydedilmiş bir yazı yüklenirken bu, blok türü için öznitelik kaynakları tarafından belirlenir. Kullanıcı bir bloğu düzenlerken bu değerler zaman içinde değişebilir ve bloğun nasıl serileştirileceğini belirlerken kullanılır.

---

## 💾 Otomatik Kaydetme (Autosave)

Yazılarınızı ve sayfalarınızı yazarken veya düzenlerken yaptığınız değişiklikler her 2 dakikada bir otomatik olarak kaydedilir. Düzenleyicinin sağ alt köşesinde, girişin en son ne zaman veritabanına kaydedildiğine dair bir bildirim görürsünüz. Otomatik kaydetme tüm yazılar ve sayfalar için otomatik olarak etkindir. Her yazı/sayfa için yalnızca bir otomatik kaydetme vardır. Her yeni otomatik kaydetme, veritabanındaki önceki otomatik kaydetmeyi üzerine yazar.

İlgili makaleler: Revision Management
Dış bağlantılar: WordPress.com Support – Autosave

---

## 👤 Avatar

Bir kullanıcıyı temsil eden grafik resim veya fotoğraftır.

Bkz.: Gravatar
İlgili makaleler: Using Gravatars
Dış bağlantılar: Avatar (computing) – Wikipedia

---

## ⚙️ Arka Uç (Back End)

Yetkili kullanıcıların giriş yaparak içerik ekleyebildiği, silebildiği veya değiştirebildiği alandır. “WordPress”, “admin” veya “yönetim alanı (administration area)” olarak da adlandırılır.

---

## 📦 İkili Dosyalar (Binaries)

Derlenmiş bilgisayar programları veya çalıştırılabilir dosyaları ifade eder. Birçok açık kaynak proje, kaynak koddan yeniden derlenebilse de, en popüler platformlar ve işletim sistemleri için önceden derlenmiş ikili dosyalar sunar.

---

## 🔲 Blok (Block)

Bir web sayfasının içeriğini veya düzenini oluşturmak için bir araya getirilen işaretleme (markup) birimlerini tanımlamak için kullanılan soyut terimdir. WordPress’te kısa kodlar (shortcodes), özel HTML ve gömülü içeriklerin birleşimini tek bir tutarlı API ve kullanıcı deneyimi içinde toplar.

---

## 📚 Blok (Ekleme) Kütüphanesi (Block Inserter Library)

Kullanılabilir blokların seçilmesi için temel arayüzdür. Bloklardaki artı simgeleri veya düzenleyici arayüzünün sol üst köşesindeki düğmelerle açılır.

---

## 🗂️ Blok Kategorileri (Block categories)

WordPress taksonomisi değildir. Bunun yerine, Blok Kütüphanesi içindeki blokları dahili olarak sıralamak için kullanılır.

---

## 🏷️ Blok Adı (Block name)

Bir blok türü için benzersiz tanımlayıcıdır. Eklentiye özgü bir ad alanı (namespace) ve bloğun amacını tanımlayan kısa bir etiket içerir.
Örn: `core/image`

---

## 🎨 Blok Stilleri (Block styles)

Blokla birlikte gelen CSS stilleridir. Bu, stil dosyasıyla veya blok işaretlemesiyle sağlanabilir. Örneğin, bloğun işaretlemesine eklenmiş bir sınıf (class), blok stillerine dâhildir.

Global Styles ile karşılaştırın. Global Styles’a karşıt olarak blok stilleri bazen Local Styles (Yerel Stiller) olarak adlandırılır.

Daha fazla bilgi için: Block Styles

---

## 🔧 Blok Destekleri (Block supports)

Blokların hangi özellikleri desteklediğini bildirmesi için kullanılan API. Bir özellik için destek bildirildiğinde, API bloğa ek öznitelikler ve çoğu mevcut blok desteği için uygun kullanıcı arayüzü kontrolleri ekler.

Bkz.: Block Supports reference documentation

---

## 🧩 Blok Şablon Parçaları (Block Template parts)

Blok Şablonlarının üzerine inşa edilen bu parçalar, WordPress sitesinde tipik olarak görülen altbilgi (Footer) veya üstbilgi (Header) gibi yeniden kullanılabilir ögelerin yapısını belirler.

Tam Site Düzenleme (Full Site Editing) ve blok tabanlı temalar ile kullanıcılar kendi şablon parçalarını oluşturabilir, bunları veritabanına kaydedebilir ve site genelinde tekrar kullanabilir. Şablon parçaları, tema şablon parçalarının blok karşılığıdır. Genellikle önce bir tema tarafından tanımlanır, semantik anlam taşır (örn. temalar arasında değiştirilebilir bir header) ve yalnızca site düzenleyici bağlamında (templates içinde) eklenebilir.

---

## 📐 Blok Şablonları (Block Templates)

Önceden tanımlı özniteliklere veya yer tutucu içeriğe sahip blok düzenleridir. Bir yazı türü için şablon tanımlayarak kullanıcılara yeni içerik oluştururken başlangıç noktası sağlayabilirsiniz.

Özünde, standart WordPress şablon hiyerarşisindeki şablonlara (örneğin index, single, archive) karşılık gelen blok işaretlemesine sahip HTML dosyalarıdır. Bu, Sayfa veya Yazı Düzenleyicisi aracılığıyla düzenlenmeyen sitenin ön uç varsayılanlarını kontrol etmeye yardımcı olur.

Bkz.: templates documentation

---

## 🎭 Blok Temaları (Block Themes)

Tam Site Düzenleme’yi (Full Site Editing) çalıştırmaya izin veren, blok temelli olarak inşa edilmiş temalardır. Temelin çekirdeğini blok şablonları ve blok şablon parçaları oluşturur. Günümüzde blok tema şablonları, standart WordPress şablon hiyerarşisindeki şablonlara karşılık gelen blok işaretlemesine sahip HTML dosyalarıdır.

---

## 🧾 Blok Türü (Block type)

Belirli bir yazıda kullanılan bloklardan farklı olarak, blok türü belirli bir blok türünün nasıl davranacağını tanımlar. Örneğin bir yazıda birçok görsel olabilir; ancak hepsi, tek bir görsel blok türü tanımına uygun şekilde davranır.

---

## 📓 Blog

Blog (veya weblog), bir kişi ya da grup tarafından çevrimiçi günlük, dergi veya düzenli olarak yayınlanan içeriktir.

Bireyler, gruplar, şirketler veya kuruluşlar tarafından kullanılabilir. Bloglar hem herkese açık hem de özel içerik barındırabilir. CMS yazılımına bağlı olarak yazarlar, bazı içeriklere hesap veya şifre aracılığıyla erişimi kısıtlayabilir.

---

## ✍️ Blog Yazarlığı (Blogging)

Bir kişinin kendi blogunda yazı yazma eylemidir. Bloglamak, bir şey hakkında blogda yazı yazmak anlamına gelir. Genellikle yazarın internette ilginç bulduğu bir şeye bağlantı vermesini de içerir.

Bkz.: Blogosphere, Blogroll

---

## 🌐 Blogosfer (Blogosphere)

İnternette bloglardan oluşan veya bloglarla ilgili web siteleri alt kümesidir.

Bkz.: Blog, Blogroll

---

## 🔗 Blogroll

Çeşitli bloglara veya haber sitelerine verilen bağlantıların listesidir. Genellikle, listedeki her siteyi izleyen ve güncelleme bilgilerini toplayarak listeyi oluşturan bir hizmet tarafından sağlanır.

WordPress’in varsayılan blogroll (bağlantılar) özelliği 3.5 sürümünde kaldırılmıştır.

Bkz.: Blog, Blogosphere, Feed, News reader
Dış bağlantılar: News aggregator – Wikipedia

---

## 📑 Bookmarklet

Bookmarklet (veya favelet), genellikle JavaScript ile yazılmış ve kullanıcıya bir işlevi gerçekleştirme olanağı tanıyan, “sahte” bir yer imi (bookmark) içerir.

Örnekler:

* delicious.com bookmarklet’leri, kullanıcıların bağlantıyı hızlıca delicious.com hesaplarına eklemelerini sağlar.
* Tantek’s favelets

---

## 🔘 Boolean

`true` veya `false` dönen değişken veya ifadedir.

Dış bağlantılar: PHP Boolean data type

---

## 🏷️ Kategori (Category)

WordPress’te her yazı bir veya daha fazla kategori altında sınıflandırılabilir. Doğru kategorilendirme, benzer içeriklerle gruplanmasını sağlar ve site içinde gezinmeyi kolaylaştırır.

Not: Yazı kategorisi, bağlantı kategorisiyle (link category) karıştırılmamalıdır. Bağlantı kategorisi, bağlantıları sınıflandırmak ve yönetmek için kullanılır.

---

## 🔐 Yetkinlikler (Capabilities)

Bir veya daha fazla türde görevi gerçekleştirme iznidir. Her WordPress kullanıcısının rolüne bağlı olarak bazı yetkinlikleri olabilir, bazıları olmayabilir.

Örneğin, Yazar (Author) rolüne sahip kullanıcılar genellikle kendi yazılarını düzenleme (`edit_posts`) yetkisine sahiptir; ancak diğer kullanıcıların yazılarını düzenleme (`edit_others_posts`) yetkisine sahip değildir.

WordPress’in rol tabanlı erişim sisteminde altı rol ve elliden fazla yetkinlik vardır. Eklentiler bu sistemi değiştirebilir.

İlgili makale: Roles and Capabilities
Dış bağlantı: Role-based access control – Wikipedia

---

## 🌉 CGI

**CGI (Common Gateway Interface)**, bir web sunucusu ile tarayıcı arasındaki iletişim için kullanılan sunucu taraflı iletişim betiklerine yönelik bir tanımdır. Genellikle formlarla veri toplayan HTML sayfaları, kullanıcı veriyi gönderdiğinde bu veriyi işlemek için CGI programlaması kullanır.

---

## 🔤 Karakter Varlığı (Character Entity)

HTML’de özel anlamı olan karakterleri göstermek için kullanılan yöntemdir.

Örn: `<` ve `>` işaretleri HTML etiket yapısında kullanıldığından, site üzerinde bu sembolleri göstermek için karakter varlıkları kullanılır:

* `<` için `&lt;`
* `>` için `&gt;`

İlgili makaleler: Fun Character Entities

---

## 🔡 Karakter Kümesi (Character Set)

Harfler, sayılar, noktalama işaretleri ve özel semboller gibi simgelerin oluşturduğu kümedir. Bilgisayarlar, bu kümedeki üyeleri sayısal bir değerle saklamak için kodlama şeması kullanır. Ek olarak, sıralama düzenini belirleyen karşılaştırma (collation) uygulanır.

Varsayılan olarak, WordPress kurulumunda oluşturulan MySQL veritabanı tablolarında **UTF-8 (utf8)** karakter kümesi kullanır. WordPress 2.2 sürümünden itibaren, veritabanı karakter kümesi (ve karşılaştırma) `wp-config.php` dosyasında tanımlanır.

Bkz.: Collation
İlgili makaleler: Editing wp-config.php, Converting Database Character Sets
Dış bağlantılar: Character set – Wikipedia, Unicode – Wikipedia, UTF-8 – Wikipedia, Character sets and collation – MySQL

---

## 🔑 chmod

**chmod**, Unix/Linux kabuk komutudur ve dosyaların izinlerini değiştirmek için kullanılır. İsmi “change mode” ifadesinin kısaltmasıdır.

İlgili makaleler: Changing File Permissions, UNIX Shell Skills, htaccess for subdirectories

---

## 🏷️ Sınıf (Class)

CSS stillerinin gruplandırılmasıdır ve herhangi bir HTML öğesine uygulanabilir.

PHP sınıfları için: Class (Computing) – Wikipedia, PHP Manual: Classes and Objects

İlgili makaleler: CSS, Blog Design and Layout

---

## 📦 Klasik Blok (Classic block)

TinyMCE editörünü bir blok olarak gömen bloktur. TinyMCE, önceki çekirdek editörün temeliydi. Blok düzenleyicisinden önce oluşturulmuş eski içerik, tek bir Classic block içine yüklenir.

---

## 📚 Codex

WordPress kullanıcılarına WordPress’i nasıl kullanacaklarını gösteren makale serisidir. WordPress kullanıcıları, Codex’e gönüllü olarak belge katkısında bulunur.

Dış bağlantılar: Codex

---

## 🔡 Karşılaştırma (Collation)

Bir karakter kümesindeki harfleri, sayıları ve sembolleri sıralamak için kullanılan düzendir. WordPress, varsayılan olarak **UTF-8 (utf8)** karakter kümesini kullandığından, kurulum sırasında oluşturulan tablolar `utf8_general_ci` karşılaştırması ile atanır. WordPress 2.2 sürümünden itibaren kullanılan karşılaştırma (ve karakter kümesi) `wp-config.php` dosyasında tanımlanır.

Bkz.: Character set
İlgili makaleler: Editing wp-config.php, Converting Database Character Sets
Dış bağlantılar: Collation – Wikipedia, Character set – Wikipedia, UTF-8 – Wikipedia, Character sets and collation – MySQL

---

## 💬 Yorumlar (Comments)

Yorumlar, okuyucuların yazılara yanıt vermesine olanak tanıyan blog özelliğidir. Genellikle okuyucular, yazının içeriği hakkında kendi düşüncelerini paylaşır; ancak bağlantı verebilir, tartışma başlatabilir veya yazarın yazısını övebilirler.

Yorumlar dil ve içerik filtreleriyle kontrol edilebilir. Görünür olmadan önce onaya alınabilir. Bu, spam yorumlarla mücadelede faydalıdır.

Bkz.: Blog
İlgili makaleler: Comment-related plugins, Dealing with comment spam, Settings Discussion SubPanel
Dış bağlantılar: Hyperlink – Wikipedia

---

## 📑 İçerik (Content)

İçerik; yazılarda paylaşılan metin, görsel veya diğer bilgileri ifade eder. Sitenin yapısal tasarımından (çerçeve) ve sunumundan (grafik tasarım) ayrıdır. Bir İçerik Yönetim Sistemi (CMS), yapısal veya grafik tasarımdan ziyade içeriğin değiştirilmesine ve güncellenmesine odaklanır.

---

## 🗂️ İçerik Yönetim Sistemi (Content Management System)

İçeriğin bakımını kolaylaştıran, ancak tasarımı değil, yazılımdır. Bir bloglama aracı, İçerik Yönetim Sistemine örnektir.

Bkz.: Blog

---

## 🖥️ cPanel

Birçok barındırma sağlayıcısının sunduğu, kullanıcıların hesaplarını kolayca yapılandırmasına imkân veren popüler bir web tabanlı yönetim aracıdır.

İlgili makaleler: Using cPanel, Adding New Themes by using cPanel
Dış bağlantılar: cPanel website

---

## 🎨 CSS

**CSS (Cascading Style Sheets)**, bir web sayfasının nasıl sunulacağını belirten, W3C açık standart programlama dilidir. Web tasarımcılarına, içeriği bağımsız olarak biçimlendirme ve düzenleme imkânı tanır.

İlgili makaleler: CSS, Blog Design and Layout
Dış bağlantılar: CSS – W3C, Open standards – Wikipedia, W3C.org

---

## 🔄 CVS

**CVS (Concurrent Versions System)**, WordPress geliştirmesini koordine etmek için kullanılan yazılımdı. Şubat 2005’ten itibaren bu işlev **Subversion (SVN)** tarafından devralınmıştır.

Daha fazla bilgi için: Using Subversion

---

## 📊 Gösterge Paneli (Dashboard)

WordPress’te Dashboard, bir sitenin (veya bir site ağı – network of sites) ana yönetim ekranıdır. Site veya ağ hakkındaki bilgileri ve ayrıca harici bilgileri, kullanıcının etkinleştirebileceği, devre dışı bırakabileceği ve yerini değiştirebileceği widget’lar aracılığıyla özetler.

İlgili makaleler: Dashboard Screen

## 🗃️ Veritabanı (Database)

Bilişimde bir veritabanı, bilgileri düzenli bir biçimde yönetmek için kullanılan yazılımdır. WordPress, blogunuzun içeriği (yazılar, yorumlar vb.) gibi verileri saklamak ve almak için **MySQL** veya **MariaDB** ilişkisel veritabanı yönetim sistemini kullanır.

İlgili makaleler: Database Description, Backing Up Your Database

---

## 🔢 Veritabanı sürümü (Database version)

WordPress’te **veritabanı sürümü**, WordPress’in verilerini veritabanında nasıl düzenlediğine dair değişiklik yapıldığında artan bir sayıdır. MySQL veya MariaDB veritabanı yazılımının sürümüyle aynı değildir.

Örneğin, WordPress 3.3’te veritabanı sürümü 19470 idi ve WordPress 3.3.1’de değişmedi. Bu, eski sürümden yedeklenmiş verileri kullanmayı planlayanlar için veri yapısında değişiklik kontrolü gerekmediğini gösterir.

WordPress, veritabanı sürümünü her WordPress sitesinin “`wp_options`” tablosunda “`db_version`” adlı seçenek olarak saklar. (Tablo adı öneki “`wp_`” bazı durumlarda olmayabilir veya farklı olabilir.)

İlgili makaleler: Database Description, How do you force a database upgrade?

---

## 🎨 Varsayılan tema (Default theme)

Her WordPress kurulumunda bir **varsayılan tema** bulunur. Varsayılan tema bazen “yedek (fallback) tema” olarak adlandırılır; çünkü etkin tema bir nedenle kaybolur veya silinirse WordPress varsayılan temayı kullanmaya geri döner.

---

## ⛔ Kullanımdan kaldırılmış (Deprecated)

**Kullanımdan kaldırılmış** fonksiyonlar veya şablon etiketleri artık desteklenmez ve yakında geçersiz olacaktır.

İlgili makaleler: “Deprecated Functions” Category

---

## 👩‍💻 Geliştirici (Developer)

**Geliştirici (dev)**, bir yazılım ürününü oluşturma, değiştirme ve güncelleme konusunda aktif olan bilgisayar programcısıdır.

İlgili makaleler: Plugin API

---

## 🧱 DIV (DIV)

HTML’de bir **DIV** öğesi bir metin bölümünü işaretler. WordPress’te, belirli blog öğelerine CSS stilleri uygulamak için DIV’ler yoğun şekilde kullanılır.

İlgili makaleler: CSS, Blog Design and Layout

---

## 🌐 DNS (DNS)

**DNS (domain name system)**, alan adlarını IP adreslerine eşleyen sistemdir. Bir tarayıcıyla bir web sitesini ziyaret ettiğinizde, tarayıcı önce URL’den alan adını çıkarır. Ardından DNS’i kullanarak bu alan adına karşılık gelen IP adresini bulur ve o IP adresine bağlanır.

Dış bağlantı: Domain Name System (Wikipedia)

---

## 🧩 DOM (DOM)

**DOM (Document Object Model)**, programcıların HTML ve XML’e dinamik olarak erişip belgelerin içeriğini ve yapısını kontrol etmesini sağlayan standart, platformdan bağımsız bir arayüzdür. DOM, programlama betikleriyle web sayfaları arasında bağlantı kurar.

Dış bağlantılar: DOM at Wikipedia, DOM at W3C.org

---

## 🏷️ Alan adı (Domain name)

**Alan adı**, internette tanımlama amacıyla kullanılan addır. WordPress’te bir alan adı genellikle WordPress’in kurulu olduğu sunucuyu tanımlar. Bunun çalışması için internetin **DNS** sistemi, alan adını bir sunucunun IP adresiyle eşler. Örneğin, `example.com` alan adı `192.0.43.10` IP adresine eşlenir. Birden çok alan adı aynı IP adresine eşlenebilir; böylece tek bir sunucu birçok web sitesini çalıştırabilir. Örneğin, `www.example.com` ve `example.net` de `192.0.43.10` IP adresine eşlenir.

Dış bağlantı: Domain name (Wikipedia)

---

## 📝 Taslak (Draft)

**Taslak** yazı durumu, kaydedilmiş ancak henüz yayımlanmamış WordPress yazıları içindir. Bir taslak yazı yalnızca **Yönetim Paneli > Yazı Yaz (Write Post) Alt Paneli** üzerinden, yazarın **Kullanıcı Düzeyi (User Level)** ile eşit veya daha yüksek düzeye sahip kullanıcılar tarafından düzenlenebilir.

---

## 🔄 Dinamik blok (Dynamic block)

İçeriği değişebilen ve bir yazı kaydedilirken önceden belirlenemeyen blok türüdür; bunun yerine yazı sitede görüntülendiğinde her seferinde hesaplanır. Bu bloklar, JavaScript uygulamalarında yedek (fallback) içerik veya hiç içerik kaydetmeyebilir; bunun yerine çalışma zamanında işleme için PHP blok uygulamasına başvurur.

---

## ✂️ Özet (Excerpt)

**Özet**, blog yazınızın kısaltılmış açıklamasıdır ve **Yönetim > Yazılar > Yeni Ekle Alt Paneli**’ndeki **Excerpt** alanına girilen metne karşılık gelir. Özet, RSS akışlarında yazınızı tanımlamak için kullanılır ve genellikle arama sonuçlarını görüntülerken kullanılır. Bazen Arşiv ve Kategori görünümlerinde de kullanılır. Bu alanın içeriğini göstermek için **Şablon Etiketi (Template Tag)** `the_excerpt()` kullanılır. Yazı yazarken **Excerpt** alanına bilgi girmez ve tema şablon dosyalarınızda `the_excerpt()` kullanırsanız, WordPress otomatik olarak yazı içeriğinin ilk 55 kelimesini görüntüler.

**Özet (excerpt)**, yazı içeriğinde `<!--more-->` öncesindeki kelimeleri ifade eden **teaser** ile karıştırılmamalıdır. Uzun bir yazı yazarken birkaç cümleden sonra `<!--more-->` **Hızlı Etiket (Quicktag)** ekleyerek bir kesme noktası oluşturabilirsiniz. Yazı görüntülendiğinde **teaser** ve ardından bir köprü (ör. “Read the rest of this entry…”) gösterilir. Ziyaretçiler bu bağlantıya tıklayarak yazınızın tam sürümünü görebilir. **Şablon Etiketi** `the_content()` teaser’ı göstermek için kullanılmalıdır.

İlgili makaleler: Customizing the Read More, Excerpt
Back to the Top

---

## 📡 Besleme (Feed)

**Besleme (feed)**, “Feedreader” yazılımlarının bir sitede yeni içerik olup olmadığını otomatik olarak kontrol edip yeni içerik ve güncellemeler hakkında bilgiyi başka bir yerde yayımlamasını sağlayan özel yazılım işlevdir. Bu, kullanıcıların farklı blog sitelerinde yayımlanan en son ve en popüler içerikleri takip etmelerini sağlar. Bazı beslemeler **RSS** (“Rich Site Summary” veya “Really Simple Syndication”), **Atom** veya **RDF** dosyalarını içerir. Feeds genellikle **XML** teknolojisine dayanır.

---

## 📥 Besleme Okuyucu (Feed Reader)

**Feedreader**’ın rolü, çeşitli web sitelerinden web beslemelerini toplayıp tek bir yerde görüntülemektir.

---

## 🧪 Süzgeç (Filter)

WordPress’te bir **Filter**, mevcut herhangi bir **Hook** belirtilerek mevcut bir **Action** ile ilişkilendirilen işlevidir.

Geliştiriciler, **Filter API**’yi kullanarak, mevcut bir Action’dan gelen kodun yerine geçecek özel Süzgeçler oluşturabilir. Bu işleme “hooking” denir.

Özel **Actions** ile özel **Filters** arasındaki fark şudur: Özel **Actions**, mevcut Action’lara kod ekleyip kaldırmanıza izin verirken; özel **Filters**, mevcut bir Action içinde bulunan belirli verilerin (ör. bir değişken) değiştirilmesini sağlar.

Bkz.: Action, Hook, Terminology Confusion
İlgili makaleler: Filters, Filter Reference, `add_filter()`

---

## 🦶 Altbilgi alanı (Footer area)

**Altbilgi alanı**, bir temanın, web sayfasının ana içeriği dışında bilgi göstermek için sağladığı yatay alandır. Temalar, içeriğin altında bir veya daha fazla altbilgi alanı sunabilir. Altbilgi alanları genellikle site yöneticisinin özelleştirebileceği **bileşenler (widgets)** içerir.

Bir temada altbilgi alanları genellikle `sidebar-footer.php` adlı şablon dosyasıyla oluşturulur.

Bkz.: Sidebar
İlgili makaleler: Templates, Customizing Your Sidebar, Stepping Into Templates, Template Hierarchy

---

## 🖥️ Ön Uç (Front End)

**Ön uç**, ziyaretçilerinizin `www.Siteniz.com` adresine geldiklerinde gördüğü ve etkileşim kurduğu kısımdır.

---

## 📤 FTP (FTP)

**FTP (File Transfer Protocol)**, dosya aktarımı için istemci-sunucu protokolüdür. Dosya indirmenin bir yolu ve sunucuya dosya yüklemenin en yaygın yoludur.

**FTP istemcisi**, bir FTP sunucusundan dosya indirebilen veya sunucuya dosya yükleyebilen programdır.

Özellikle bir barındırma sağlayıcısı kullanıyorsanız, WordPress dosyalarınızı web sunucunuza yüklemek için bir FTP istemcisi kullanmanız gerekebilir.

İlgili makaleler: FTP Clients, Uploading WordPress to a remote host, Using FileZilla

---

## 🧱 Tam Site Düzenleme veya FSE (Full Site Editing or FSE)

Bu, kullanıcıların tüm web sitelerini blokları başlangıç noktası olarak kullanarak düzenlemesine olanak tanıyan özellikler bütününü ifade eder. Bu özellik seti, blok desenlerinden (block patterns) global stillere, şablonlardan bloklar için tasarım araçlarına (ve daha fazlasına) kadar her şeyi içerir. İlk olarak WordPress 5.9’da yayımlandı.

---

## 🖼️ Galeri (Gallery)

Andy Skelton tarafından tanımlandığı şekliyle, WordPress 2.5 ile tanıtılan **Galeri**, bir yazıya ekli görsellerin sergilenmesidir. Benzer şekilde, bir yükleme, bir yazıyı düzenlerken yüklediğinizde “yazıya ekli” kabul edilir.

Yükleyicide, düzenlemekte olduğunuz yazıya ekli tüm yüklemeleri gösteren bir “Gallery” sekmesi vardır. Bir yazıda birden fazla ekiniz olduğunda, Gallery sekmesinin altında “Insert gallery” adlı bir düğme görmelisiniz. Bu düğme, yazıya bir kısa kod (**shortcode**) ekler. WordPress, bu kısa kodu o yazıya ekli tüm görsellerin sergisiyle değiştirir. Görsel olmayan dosya türleri galeriye dâhil edilmez.

Not: “Insert gallery” düğmesini görmüyorsanız, bunun sebebi yazıya iki görsel eklememiş olmanız olabilir.

Ekler için “pretty URL”ler yalnızca yazıyı yayımladıktan sonra oluşturulur ve yazı kalıcı bağlantısı (permalink) artı ek “slug”’ından oluşmalıdır.

İlgili makaleler: Gallery Shortcode, Shortcode API

---

## 🌍 gettext (gettext)

**gettext** sistemi, WordPress’in birçok dilde sürüm sunmasını sağlayan çeviri araçları ve standartları bütünüdür. WordPress’te çeviri için bir metin dizesinin “alanı (domain)” ve “bağlamı (context)” olabilir. Örneğin, bir eklenti çevirileri için kendi alanını belirtebilir; bağlam ise kullanıcı arayüzünün farklı bölümlerinde aynı İngilizce kelime veya ifadeye farklı çeviriler yapılmasına yardımcı olur.

İlgili makaleler: WordPress in Your Language, Translating WordPress, I18n for WordPress Developers
Dış bağlantılar: gettext (Wikipedia), GNU gettext

---

## 🕰️ GMT (GMT)

**GMT (Greenwich Mean Time)**, diğer tüm saat dilimlerinin ölçüldüğü eski saat diliminin adıdır ve Greenwich, İngiltere’deki Kraliyet Gözlemevi’ndeki zamana karşılık gelir. Yerini **UTC (Universal Time, Coordinated)** almıştır; ancak pratikte UTC ve GMT çoğu durumda aynı kabul edildiğinden “GMT” terimi hâlâ yaygın şekilde kullanılır.

Dış bağlantılar: Greenwich Mean Time, Time zone, UTC (Wikipedia)

---

## 👤 Gravatar (Gravatar)

**Gravatar**, küresel olarak tanınan bir avatar’dır (kullanıcıyı temsil eden grafik resim/fotoğraf). Genellikle bir kullanıcının gravatar’ı e-posta adresiyle ilişkilendirilir ve **Gravatar.com** gibi bir hizmet kullanılarak yönetilir. Site sahibi, yorumlarla birlikte kullanıcının gravatar’ının gösterilecek şekilde sitesini yapılandırabilir.

Bkz.: Avatar
İlgili makaleler: How to Use Gravatars in WordPress, Using Gravatars
Dış bağlantılar: Gravatar at Wikipedia

## 🖥️ Grafik Kullanıcı Arayüzü (GUI – Graphical User Interface)

GUI (“gooey” şeklinde telaffuz edilir), kullanıcıların fareyi veya imleci grafik simgelere yönelterek etkileşim kurmasını sağlayan arayüzdür.

---

## 🧱 Gutenberg (Gutenberg)

Gutenberg, yeni geliştirilmiş, blok odaklı düzenleyicidir. WordPress’i özelleştirmenin tutarsız bir düzine yolunun yerine **bloklar (blocks)** kullanarak her tür içeriği oluşturur; modern kodlama standartlarıyla uyum sağlar ve açık web girişimleriyle hizalanır. Bu içerik blokları, teknik yeterlilikten bağımsız olarak herkes için yayıncılığı — ve işi — demokratikleştirerek kullanıcıların, geliştiricilerin ve barındırma sağlayıcılarının WordPress ile etkileşimini dönüştürür; zengin web içeriği oluşturmayı daha kolay ve sezgisel hâle getirir.

---

## 🛠️ Hack (Hack)

Hack, bir yazılım ürününün işlevselliğini özelleştirmek veya genişletmek için yazılmış küçük bir koddur. WordPress’in eski sürümleri hack tabanlı bir genişletme sistemi kullanıyordu; ancak 1.2 ve üzeri sürümler, eklentiler için kancalar (hooks) içeren **Eklenti API’si (Plugin API)** kullanır.

Bkz.: Hacking, Plugin
İlgili makaleler: Changelog, Plugin API
Dış bağlantılar: Open source – Wikipedia

---

## 💻 Hackleme (Hacking)

Hacking, bir yazılım için kod yazma veya ona kod katkısında bulunma sürecidir.

Terimin anlamı konusunda bazı tartışmalar vardır. Başlangıçta “ustalık sergilemek” veya “değiştirmek/iyileştirmek” anlamına gelen zararsız bir terimken, popüler medya tarafından “kötü niyetle bir bilgisayar sistemine izinsiz girmek” şeklinde yorumlanmıştır. Sektörde birçok kişi, terimi asıl anlamıyla geri kazanmak isterken, kötü niyetli yorumu ifade etmek için **cracking** terimini benimsemiştir. Bu nedenle, özellikle açık kaynak projelerinde “hacking” sözcüğü çoğunlukla zararsız anlamıyla kullanılır. Terimin tarihi için Wikipedia’daki **Hacker** makalesine bakınız.

Bkz.: Hack
İlgili makaleler: Plugins

---

## 🖼️ Üstbilgi Görseli (Header Image)

Header Image, bir WordPress web sitesinin en üstünde görünen geniş resimdir.

---

## 🧷 Kanca (Hook)

Hook’lar, geliştirici tarafından **Actions** ve **Filters** içinde belirtilir. WordPress’te mevcut tüm Hook’ların (umarız) tam listesi mevcuttur.

Actions ve Filters tarafından kullanıldıkları için zaman zaman “Action Hooks” ve “Filter Hooks” ifadelerini duyabilirsiniz.

Teknik ve katı terimlerle: Bir **Hook**, **do\_action()** veya **apply\_filters()** çağrılarıyla tetiklenen bir “olaydır” (Observer desenindeki event). Bu çağrılar, önceden **add\_action()** veya **add\_filter()** ile o olaya bağlanmış tüm action veya filter işlevlerini çalıştırır.

Bkz.: Action, Filter
İlgili makaleler: Hooks, Actions and Filters, Plugin API/Hooks

---

## 🧩 Terminoloji Karışıklığı (Terminology Confusion)

WordPress Codex ve kaynak kod yorumlarında, bazen “actions/filters” ve “hooks” terimleri karıştırılmaktadır.

Actions, Filters ve Hooks; bazen “action/filter hooks” veya “action/filter/hook functions” olarak da anılır.

---

## 🏢 Barındırma Sağlayıcısı (Hosting provider)

Barındırma sağlayıcısı, genellikle ücret karşılığında, bilgilerin web üzerinden erişilebilir olmasını sağlayan altyapı sunan şirket/kuruluştur. Bu; bir web sunucusunun (Apache gibi web sunucu yazılımı dahil) kullanımını ve FTP, PHP, MySQL veya MariaDB gibi ilgili teknolojileri ile Linux veya Unix gibi işletim sistemlerini içerebilir.

İlgili makaleler: Hosting WordPress

---

## ⚙️ .htaccess (.htaccess)

`.htaccess`, **Apache** web sunucusu yazılımı için, bulunduğu dizin ve/veya alt dizinleri özelinde sunucu yapılandırma ayarlarını belirlemek/değiştirmek amacıyla kullanılan ayrıntılı bir yapılandırma dosyasıdır.

WordPress, kalıcı bağlantılar (permalinks) üretmek için `.htaccess` dosyasını **mod\_rewrite** Apache modülü ile birlikte kullanır.

`.htaccess`, Unix/Linux’ta gizli bir dosyadır (başındaki nokta ‘.’ nedeniyle). Bu nedenle bazı FTP istemcilerinin varsayılan ayarlarında görünmeyebilir.

Bkz.: chmod
İlgili makaleler: htaccess for subdirectories, Using Permalinks, UNIX Shell Skills, Changing File Permissions

---

## 🧾 HTML (HTML – Hypertext Markup Language)

**HTML**, web sayfalarının anlamsal içeriğini tanımlamak için kullanılan işaretleme dilidir. Genellikle **CSS** ve/veya **JavaScript** ile birlikte kullanılır. WordPress, web sayfalarını **HTML5** standardına uygun olarak üretir. Standart, **World Wide Web Consortium (W3C)** tarafından belirlenir.

---

## 🧰 Tümleşik Geliştirme Ortamı (IDE – Integrated Development Environment)

Bir IDE, yazılım geliştirme için çeşitli araçlar sağlayan bir uygulamadır. Genellikle şunları içerir:

* kaynak kod düzenleyici (Text Editor benzeri)
* hata ayıklayıcı (WordPress bağlamında PHP ve JavaScript için yararlıdır)
* otomatik derleyici/oluşturucu (automated builder)

Önerilen IDE’lerimiz için **Editing Files** sayfasına bakınız.

---

## 🧪 Denetleyici (Inspector)

Kullanımdan kaldırılmış terim. **Settings Sidebar**’a bakınız.

---

## 🌐 IP adresi (IP address)

**IP adresi**, bir bilgisayara (veya ağ yazıcısı gibi internet özellikli başka bir cihaza) atanan, diğer cihazlarla **Internet Protocol** kullanarak iletişimi mümkün kılan benzersiz bir sayıdır (örn. `70.84.29.148`). İnternetteki kimliktir; internete bağlı her bilgisayara en az bir IP adresi atanır. Atama yöntemi, kalıcılığı ve süresi kullanım amacına ve koşullara göre değişebilir.

Her web sunucusunun da bir IP adresi vardır; ancak barındırma sağlayıcıları, aynı fiziksel sunucuda birden çok web sitesi barınıyorsa tek bir bilgisayara birden çok IP adresi atayabilir. Bu, çoğu ekonomik “yönetimli” veya “grup” barındırma paketinde yaygındır.

Alan adları, IP adreslerinin yazımı zahmetli ve hatırlaması güç olduğu için, internet kaynaklarına erişimi kolaylaştırmak amacıyla oluşturulmuştur. Her alan adının en az bir IP adresi karşılığı vardır; ancak yalnızca sunucular alan adına ihtiyaç duyduğundan, çok az IP adresinin bir alan adı bulunur. **DNS**, alan adlarını IP adreslerine eşleyen sistemdir.

Dış bağlantılar: IP address – Wikipedia

---

## 🧩 ISAPI (ISAPI – Internet Server Application Programming Interface)

ISAPI, verimli web tabanlı uygulamaları hızlı ve kolay geliştirmek için tasarlanmış programlama standartları kümesidir. **Process Software** ve **Microsoft** tarafından geliştirilmiş olup **CGI** programlarının yerine geçmesi amaçlanmıştır.

Dış bağlantılar: ISAPI – Wikipedia

---

## 🟨 JavaScript (JavaScript)

**JavaScript**, sunucunun yapmasının uygun olmadığı veya mümkün olmadığı durumlarda, web tarayıcınızda belirli işlemlerin yapılmasını sağlayan programlama dilidir. Örneğin, bir WordPress blogunda bir yoruma yanıt verdiğinizde, WordPress yanıt formunu yanıtladığınız yorumun içine taşımak için JavaScript kullanır.

Bkz.: AJAX, HTML, XHTML
İlgili makale: Using Javascript
Dış bağlantı: JavaScript – Wikipedia

---

## 🐧 Linux (Linux)

**Linux**, **Linus Torvalds** tarafından oluşturulan, Unix benzeri açık kaynaklı bir işletim sistemidir. Web sunucuları ve diğer yüksek performanslı bilgi işlem ortamlarında popülerdir; son yıllarda iş istasyonlarında da yaygınlaşmaktadır.

Dış bağlantılar: Linux at Shortopedia

---

## 🎨 Yerel Stiller (Local Styles)

Bkz.: **Block Styles**.

---

## 🍎 Mac OS X (Mac OS X)

**Mac OS X**, modern Macintosh bilgisayarları için özel olarak geliştirilmiş bir işletim sistemidir. 2001’de ticari olarak yayımlanmıştır. İki ana bileşenden oluşur: **Darwin** (BSD kaynak ağacına ve Mach mikro çekirdeğine dayanan, Apple tarafından geliştirilen açık kaynaklı Unix benzeri ortam; bağımsız geliştiricilerin katkılarıyla) ve **Aqua** (Apple tarafından geliştirilen tescilli grafik kullanıcı arayüzü).

İlgili makaleler: UNIX Shell Skills

---

## 🐬 MariaDB (MariaDB)

**MariaDB**, **MySQL** ilişkisel veritabanı sisteminin, MySQL’in orijinal geliştiricilerinin çoğu tarafından oluşturulan bir çatallanmasıdır (fork). WordPress ile aynı derecede uyumlu şekilde çalışır.

---

## 🧭 Menü (Menu)

Menüler, WordPress sitelerinde görünen sayfa ve yazılara bağlantı veren bağlantı listeleridir.

---

## 🏷️ Meta (Meta)

Meta’nın birden çok anlamı vardır; genel olarak “hakkında bilgi” demektir. WordPress’te meta genellikle idari türde bilgiyi ifade eder. **Meta Tags in WordPress**’te açıklandığı üzere **meta**, bir web sayfasını dış dünyaya (arama motorlarına) tanımlamak için kullanılan HTML etiketidir. **Post Meta Data** makalesinde meta, her yazıyla ilişkili yazar adı, yayımlanma tarihi gibi bilgileri ifade eder. **Meta Rules**, Codex’i kullanırken izlenecek genel protokolü tanımlar. Ayrıca birçok WordPress tabanlı sitede, genellikle kenar çubuğunda (sidebar) bulunan ve o sitede oturum açma/kayıt bağlantılarını içeren bir **Meta** bölümü bulunur. Son olarak, Meta; Codex içindeki yönetim işlevlerine atıfta bulunan bir **MediaWiki ad alanıdır (namespace)**.

Dış bağlantılar: Wikipedia’s Article on Meta

---

## 🔖 Mikroformatlar (Microformats)

Mikroformatlar, web sayfalarını insanlar için görünürde değiştirmeden, belirli bilgilerin programlar tarafından okunabilmesini sağlar. İnsanlar tarafından daha iyi tanınan web içeriğinin belirli kısımlarının anlamını programların da anlayabilmesi için genel HTML işaretlemesine anlamsal bilgi eklerler. Örneğin, bir kullanıcının profilini görüntüleyen bir web sayfası, programların kullanıcının iletişim bilgilerini kolayca ayıklayıp tek işlemle bir adres defterine eklemesini sağlamak için mikroformatlar kullanabilir. WordPress’te bazı temalar ve eklentiler belirli mikroformatları destekler.

İlgili: Themes and plugins providing microformats support
Dış bağlantılar: Microformats.org

---

## ✉️ MIME (MIME – Multipurpose Internet Mail Extension)

**MIME**, e-postanın biçimini aşağıdakileri destekleyecek şekilde genişleten bir internet standardıdır:

* ASCII dışındaki karakter kümelerinde metin
* Metin olmayan ekler
* Birden çok parçalı mesaj gövdeleri
* ASCII olmayan karakter kümelerinde üstbilgi bilgisi

MIME’ın kullanımı e-posta içeriğinin tanımlanmasının ötesine geçmiştir; artık web dâhil genel anlamda içerik türünü tanımlamak ve bazı ticari ürünlerde zengin içerik depolamak için de sıkça kullanılır.

Dış bağlantılar: IANA Media Types Specification, Wikipedia

---

## 📱 Mobil Bloglama (Moblogging)

**Moblogging**, bir mobil cihaz (örn. cep telefonu, akıllı telefon veya tablet) aracılığıyla bir bloga gönderi yayımlama eylemidir. “mōbə-logging” veya “mōb-logging” şeklinde, bazen de **smart mobs**’a atfen “mŏb-logging” olarak telaffuz edilir.

İlgili makaleler: Moblog Clients, Post to your blog using email

---

## 🔁 mod\_rewrite (mod\_rewrite)

**mod\_rewrite**, **Apache** web sunucusunun istek anında URL “yeniden yazımı”nı sağlayan bir eklenti modülüdür. Yeniden yazım kuralları (rewrite rules), istemciden gelen istenen URL’yi düzenli ifadelerle (regular expressions) çözümleyip farklı bir URL’ye çevirir ve bu yeni URL’nin içeriğini orijinal URL altında sunar veya istemciyi yeni URL’yi istemeye yönlendirir.

WordPress, kalıcı bağlantı (permalink) yapısı ve (opsiyonel bir işlev olan) çoklu site ağları (multisite networks) için **mod\_rewrite** kullanır.

İlgili makaleler: Using Permalinks, Create A Network

---

## 🕸️ Çoklu Site (Multisite)

**Multisite**, WordPress 3.0 ve sonrası sürümlerde, birden çok sanal sitenin tek bir WordPress kurulumunu paylaşmasını sağlayan özelliktir. Multisite etkinleştirildiğinde, özgün WordPress sitesi bir site ağını (network) destekleyecek şekilde dönüştürülebilir.

İlgili makale: Create A Network

## 🐬 MySQL (MySQL)

MySQL, Windows, Unix/Linux ve Mac OS X dâhil birçok platformda kullanılabilen, yaygın bir açık kaynak SQL (Structured Query Language) veritabanı uygulamasıdır.

WordPress, yazılar, yorumlar, üstveriler (metadata) ve diğer bilgiler dâhil olmak üzere tüm blog bilgilerini depolamak için bir MySQL veritabanı gerektirir.

WordPress ayrıca **MariaDB (MariaDB)** ve **Percona Server (Percona Server)** gibi MySQL uyumlu veritabanlarıyla da çalışır.

İlgili makaleler: Database Description
Dış bağlantılar: MySQL, MariaDB, Percona Server

---

## 🧭 Gezinme (Navigation)

Gezinme, bir sayfadaki seçildiğinde web sitesinin başka bir yerindeki ilgili bir sayfaya yönlendiren metni tanımlamak için kullanılan terimdir. Bazen menü, bağlantılar (links) veya köprüler (hyperlinks) olarak da adlandırılabilir.

---

## 🧭 Gezinme Bloğu (Navigation Block)

Bir sitenin gezinme menüsünü, hem yapı hem de tasarım açısından düzenlemenizi sağlayan bloktur.

---

## 🕸️ Ağ (Network)

WordPress kullanıcı arayüzünde **ağ (network)**, çoklu site (multisite) özelliğiyle tek bir WordPress kurulumunda oluşturulan ayrı siteler koleksiyonudur. Bir WordPress ağındaki siteler, diğer ağ türlerindeki varlıklar gibi birbirine bağlı değildir; WordPress.com’daki ayrı bloglara benzerler.

WordPress kodunda **network** “site”, **sites** ise “blogs” olarak adlandırılır.

İlgili makaleler: Create A Network

---

## 📰 Haber Okuyucu (News reader)

Haber toplayıcı (news aggregator) veya haber (feed) okuyucu, RSS, RDF veya Atom aracılığıyla dağıtılan bilgi beslemelerini izleyen bir bilgisayar programıdır. Çoğu haber toplayıcı, bir beslemeye “abone” olmanıza ve e-posta istemcilerinin okunan e-postaları izlemesine benzer şekilde, okuduğunuz makaleleri otomatik olarak takip etmenize olanak tanır.

Birçok blog, haber toplayıcılar kullanan okuyucuların rahatlığı için içeriklerini besleme biçiminde sunar. WordPress, RSS ve/veya Atom formatlarında beslemeler oluşturabilir.

Dış bağlantılar: News aggregator at Wikipedia

---

## 🔐 Tek Seferlik Jeton (Nonce)

**Nonce**, beklenmeyen veya yinelenen isteklerin işlenmesini önlemek amacıyla güvenlik için kullanılır; aksi hâlde bunlar web sitesinde, özellikle veritabanında istenmeyen kalıcı ya da geri döndürülemez değişikliklere yol açabilir. Özellikle, **nonce**, bir web sitesi tarafından gelecekte o siteye yapılacak istekleri tanımlamak için üretilen tek kullanımlık bir belirteçtir. Bir istek gönderildiğinde, web sitesi bu tür bir istek için daha önce üretilmiş beklenen bir nonce’ın gönderilip gönderilmediğini doğrular ve isteğin güvenle işlenip işlenemeyeceğine veya başarısızlık bildirimine karar verir. Bu, istenmeyen, süresi geçmiş veya kötü niyetli isteklerin işlenmesini engelleyebilir.

Nonce genellikle gizli bir HTML form alanında veya bir URL’nin parçası olarak bulunur ve böylece bir formu göndererek veya bir bağlantıyı ziyaret ederek istekle birlikte gönderilir. Bir istek doğrulanmazsa, web sitesi yanıtında yeni bir nonce üretebilir ve kullanıcının isteği bilerek yeniden onaylamasını isteyebilir. WordPress’te varsayılan yanıt iletisi “Are you sure you want to do this?” şeklindedir.

İlgili makaleler: WordPress Nonces

---

## 🧑‍💻 Açık Kaynak (Open Source)

**Açık kaynak (open source)**, isteyen herkesin okuyabildiği, görüntüleyebildiği, değiştirebildiği ve dağıtabildiği programlama kodudur. WordPress, açık kaynak **GNU General Public License (GPL)** kapsamında dağıtılır.

İlgili makaleler: GPL, License
Dış bağlantılar: Open Source Initiative, Open Source at Wikipedia, Source Code at Wikipedia

---

## ⚙️ Seçenekler (Options)

**Seçenekler (Options)**, WordPress’in çeşitli tercihleri ve yapılandırma ayarlarını depolamak için kullandığı veri parçalarıdır. Veritabanında veri depolamanın basit ve standart yolu olan **Options API (Options API)** kullanılarak, seçenekler `wp_options` tablosundan eklenebilir, değiştirilebilir, kaldırılabilir ve alınabilir.

İlgili makaleler: Option Reference, Transients API, Options API

---

## 🗜️ Çıktı Sıkıştırma (Output Compression)

**Çıktı sıkıştırma (output compression)**, HTML belgenizden boşlukların, satır sonlarının, yeni satırların ve sekmelerin kaldırılması işlemidir. Bu, işlevselliği değiştirmeden HTML belgesinin dosya boyutunu azaltır.

İlgili makaleler: Output Compression

---

## 📄 Sayfa (Gönderi türü) (Page (post type))

**Sayfa (Page)**, genellikle kendiniz veya siteniz hakkında “statik” bilgi sunmak için kullanılır. Örneğin **Hakkında (About)** sayfası. **Sayfa**, zamana bağlı nesneler olan **yazılar (posts)** ile karıştırılmamalıdır. Sayfalar genellikle “zamandan bağımsızdır” ve blogunuzun “dışında” yaşar.

“page” sözcüğü uzun süredir web’deki herhangi bir HTML belgesini tanımlamak için kullanılmıştır. Ancak WordPress’te **“Page”**, ilk kez WordPress 1.5 sürümünde tanıtılmış çok spesifik bir özelliği ifade eder.

İlgili makaleler: Pages, Write Page SubPanel

---

## 🧩 Desenler (Patterns)

WordPress 6.3, **Yeniden Kullanılabilir Bloklar (Reusable Blocks)** adını **Desenler (Patterns)** olarak değiştirdi. **Senkronize (synced) bir desen**, yeniden kullanılabilir blok ile aynı şekilde davranır.

Desenler, kullanıcı tarafından her seferinde değiştirilmesi amaçlanan, başlangıç içeriği olarak eklenebilen blok düzenleridir. Eklendikten sonra yerel bir kayıt olarak var olurlar ve küresel değildirler.

İlgili makaleler: Patterns, Comparing Patterns to Template Parts.

---

## 🐪 Perl (Perl)

**Perl**, “Practical Extraction and Report Language” kısaltmasıdır ancak çoğunlukla özel isim gibi yazılır. Web uygulamalarında kullanılan, çok popüler ve güçlü bir betik dilidir; yine de ana akımda kullanımı büyük ölçüde **PHP** ile yer değiştirmiştir. Güçlü yönlerinden biri, düzenli ifadeleri hızlı ve etkili kullanmasıdır. Resmî olmayan sloganı, sözdiziminin aşırı esnekliği nedeniyle “There’s More Than One Way To Do It (TMTOWTDI)”’dir.

WordPress **Perl** kullanmaz; bu nedenle Perl gerektirmez.

---

## 🔗 Kalıcı Bağlantı (Permalink)

**Kalıcı bağlantı (permalink)**, bir kaynağın veya makalenin kalıcı olarak bulunacağı URL’dir. CMS tabanlı birçok sayfa, sıkça değişen içerik özetleri barındırır; bu da içlerindeki bilgilere bağlantı vermeyi zorlaştırır. Kalıcı bağlantılar, kullanıcıların değişmeyeceğini bildikleri ve her zaman aynı içeriği sunacakları bir URL’de tam makaleleri yer imlerine eklemelerini sağlar.

Kalıcı bağlantılar WordPress’te isteğe bağlıdır, ancak URL’lerin temizliğini önemli ölçüde artırdıkları için şiddetle önerilir. WordPress, kalıcı bağlantı sistemini uygulamak için **Apache modülü mod\_rewrite (mod\_rewrite)** kullanır.

İlgili makaleler: Using Permalinks
Dış bağlantılar: URL at Wikipedia

---

## 🔒 İzinler (Permissions)

**İzinler (permissions)**, kullanıcıların belirli işlevleri yapmasını kısıtlayan veya onlara izin veren güvenlik ayarlarıdır. Unix veya Linux sistemlerindeki dosyalar için üç tür izin vardır: okuma (read), yazma (write) ve çalıştırma (execute). **MySQL/MariaDB** veritabanlarında ise çok daha fazlası vardır: **SELECT, INSERT, UPDATE, DELETE** vb. — gerçi MySQL/MariaDB bunları **ayrıcalıklar (privileges)** olarak adlandırır.

İlgili makaleler: Changing File Permissions

---

## 🟨 PHP (PHP)

**PHP (PHP: Hypertext Preprocessor)**, özellikle HTML ile bütünleşme için tasarlanmış, popüler bir sunucu tarafı betik dilidir ve (genellikle **MySQL** veya **MariaDB** ile birlikte) İçerik Yönetim Sistemleri ve diğer web uygulamalarında kullanılır. Windows, Unix/Linux ve Mac OS X dâhil birçok platformda mevcuttur ve açık kaynak yazılımdır.

WordPress, **PHP** ile yazılmıştır ve çalışması için PHP gereklidir.

Dış bağlantılar: PHP Website, PHP for Designers — by WordPress lead developer Matthew Mullenweg, PHP at OnLAMP

---

## 🧰 phpMyAdmin (phpMyAdmin)

**phpMyAdmin**, **MySQL** veya **MariaDB** veritabanlarını yönetmek için web tabanlı, güçlü ve popüler bir arayüzdür. PHP ile yazılmış açık kaynaklıdır ve MySQL/MariaDB ile çalışmak için mevcut en iyi araçlardan biridir.

İlgili makaleler: phpMyAdmin
Dış bağlantılar: phpMyAdmin web site

---

## 📡 Ping (Ping)

WordPress arayüzünde “ping”, bazen **Pingbacks** ve **Trackbacks**’i ifade etmek için kullanılır.

Genel bilgisayar terimi olarak “ping”, bir TCP/IP ortamında belirli bir IP adresinin var olup olmadığını veya erişilebilir olup olmadığını belirlemek için kullanılan yaygın bir yardımcı programdır. Genellikle ağ bağlantısı sorunlarını teşhis etmek için kullanılır. Sıklıkla “Bu adresi ping’leyebiliyor musun?” diye sorulur; bu, “ping” aracının “sorunlu” IP adresine ulaşmaya çalıştığında başarı dönüp dönmediğini ifade eder.

Dış bağlantılar: Ping at Wikipedia

---

## 🔁 Geri Bildirim Bağlantısı (Pingback)

**Pingback**, bir makaleye (blog yazısına) bağlantı verdiğinizde, o makalenin yazarını haberdar etmenizi sağlar. Yazınızda verdiğiniz bağlantılar pingback etkin bir bloga işaret ediyorsa, o blogun yazarı, makalesine bağlantı verdiğinize dair bir pingback bildirimi alır.

Gerçekten teknik detaya girmek isterseniz **Pingback teknik belirtimi**ni veya Otto’nun “How Pingbacks Work” açıklamasını inceleyebilirsiniz.

Bkz.: Trackback
İlgili makaleler: Introduction to Blogging: Pingbacks


## 🧩 Eklenti (Plugin)

Bir **Eklenti (Plugin)**, standart bir WordPress blogunda mevcut işlevselliği genişletebilen PHP fonksiyonları grubudur. Bu fonksiyonlar tek bir PHP dosyasında tanımlanabileceği gibi birden fazla dosyaya da dağıtılabilir. Genellikle, bir eklenti, WordPress’i kurduğunuz web sunucunuzdaki “`wp-content/plugins`” dizinine yükleyebileceğiniz bir PHP dosyasıdır. Eklenti dosyasını yükledikten sonra, blogunuzun yönetim arayüzündeki “Plugins” sayfasından eklentiyi “açabilir” veya etkinleştirebilirsiniz. WordPress kaynak kodu, eklentiler tarafından kullanılabilecek **hooks** içerir.

Bkz.: Hack, Hacking
İlgili makaleler: Plugins

---

## 🔁 Taşıma (Port)

WordPress topluluğu bağlamında **port (taşıma)**, WordPress ile uyumlu olacak şekilde yeniden yazılmış küçük bir kod parçasıdır. Örneğin, biri MoveableType için bir eklenti yazdıysa, WordPress kullanıcıları bu eklentinin WordPress’e **port** edilmiş sürümünü bulmak isteyebilir. **Port** fiil olarak da kullanılır: Bir yazılımı başka bir platform/dil için yeniden yazmak.

Dış bağlantılar: Porting – Wikipedia

---

## 📝 Yazı (Post)

“Makale (articles)” olarak da bilinir ve bazen yanlışlıkla “bloglar” olarak adlandırılır. WordPress’te “**posts (yazılar)**”, blogunuzu doldurmak için yazdığınız makalelerdir.

---

## ⚙️ Yazı Ayarları (Post settings)

Zamanlama, görünürlük, terimler ve öne çıkarılmış görsel dâhil yazıya ait üstveri (metadata) alanlarını içeren kenar çubuğu bölgesidir.

---

## 🔖 Yazı Kısaltması (Post Slug)

Bir yazıyı tanımlayan ve genellikle URL dostu (okunabilir ve kafa karıştırıcı karakterler içermeyen) kalıcı bağlantı oluşturmak üzere yazı başlığından türetilmiş, tirelerle ayrılmış birkaç küçük harfli kelimedir. **Post slug**, özel kalıcı bağlantı yapısında “`%posttitle%`” yer tutucusunun yerine geçer. **Post slug** değiştirilmemelidir; özellikle başlık uzun ya da sık değişiyorsa faydalıdır.

---

## 🏷️ Yazı Durumu (Post Status)

Yönetim Paneli’ndeki **Write Post SubPanel** üzerinden ayarlanan yazı durumudur: **Published** (herkes tarafından görülebilir), **Draft** (yazarın kullanıcı düzeyiyle eşit veya daha yüksek seviyedeki herkes tarafından görülebilen tamamlanmamış yazı) veya **Private** (yalnızca Yönetici düzeyindeki WordPress kullanıcıları tarafından görülebilir).

İlgili makaleler: Post Status

---

## 🧱 Yazı Türü (Post Type)

**Post type**, WordPress’in **posts** tablosunda tutulan çeşitli yapılandırılmış veri türlerini ifade eder. Yerleşik (native) kayıtlı yazı türleri: **post, page, attachment, revision, nav-menu-item**. WordPress, **register\_post\_type()** ile tanımlanabilen **özel yazı türlerini (custom post types)** de destekler. Özel yazı türleri; portföyler, projeler, video kütüphaneleri, podcast’ler, alıntılar, sohbetler ve kullanıcı veya geliştiricinin hayal edebileceği diğer içeriklerin kolayca oluşturulup yönetilmesini sağlar.

İlgili makaleler: Post Types

---

## 🔍 Sorgu (Query)

Perde arkasındaki süreçtir. Aşağıya bakınız. 🙂

İlgili makaleler: Query Overview, Custom Queries, WP Query, WP User Query
Bkz.: query string, query variable

---

## 🧰 Sorgu Bloğu (Query Block)

Klasik **WP\_Query**’yi yineleyen ve ek işlevlerle daha ileri düzey özelleştirmeye izin veren bloktur.

---

## 🧵 Sorgu Dizesi (Query String)

Bir web sayfasının hangi dinamik verileri görüntüleyeceğini belirlemek için kullanılan URI içindeki kod dizisidir. URI’deki sorgu dizesi, ilk soru işaretinden sonra gelir ve & işaretiyle ayrılmış birden fazla parametre içerebilir. WordPress, veritabanında belirli yazıları veya yazı kümelerini aramak için ölçütleri belirtmek amacıyla sorgu dizelerini kullanır. Sorgu dizelerinin kullanımı, arama motorlarının dinamik sayfaları dizine eklemesini engelleyebileceği düşüncesi yaygındır. Bu nedenle, sorgu dizelerini arama motorlarına ve ziyaretçilere daha az maruz bırakmak için **mod\_rewrite** gibi yöntemler tercih edilir.

---

## 🧮 Sorgu Değişkeni (Query Variable)

Sorgu dizesiyle iletilen değişkendir. Örneğin, `?category_name=tech&feed=atom` sorgu dizesinde iki sorgu değişkeni vardır: **category\_name** değeri “tech”, **feed** değeri “atom”.

---

## ⚡ QuickTag (QuickTag)

**QuickTag**, yazılarınıza HTML kodu ekleyen bir kısayol veya tek tık düğmesidir. `<em>` (emphasis) ve `</em>` (stop emphasis) HTML etiketleri **QuickTag** örnekleridir. `<!–contactform–>` gibi bazı **QuickTag**’ler, eklentiler tarafından metni değiştirmek veya belirli işlemleri gerçekleştirmek için kullanılan HTML yorum (comment) kodu ekler.

---

## 🧩 RDF (RDF)

**Resource Description Framework**. Web üzerindeki kaynakların konumlarını tanımlamak için kullanılan bir dildir. WordPress, yazıların konumlarını tanımlayan RDF biçiminde çıktı üretebilir. **RSS** gibi, RDF de içerik yayılımı (syndication) için kullanılır.

---

## 📚 Kayıt Kümesi (Recordset)

Bir veritabanı sorgusundan dönen kayıt grubunu veya sonucu ifade eder.

Bkz.: MySQL, **wpdb** veritabanı sınıfı

---

## 📁 Göreli Yol (Relative Path)

**Göreli yol (relative path)**, bir dosyanın, mevcut çalışma dizinine göre konumudur ve eğik çizgi (`/`) ile başlamaz. Bu, tam konumu veren **mutlak yoldan (absolute path)** farklıdır.

Bkz.: Absolute Path
Dış bağlantılar: Path\_Computing – Wikipedia

---

## 🔗 Göreli URI (Relative URI)

**Göreli URI (relative link)**, bir temel URI’ye göre yorumlanan (çözümlenen) kısmi URI’dir.

World Wide Web’de iki biçimde görülür:

Bir **mutlak yola** sahip göreli URI, alan adı köküne göre yorumlanır:
`/images/icecream.jpg` → `http://domain.example/images/icecream.jpg`

Bir **göreli yola** sahip göreli URI, mevcut belgenin URL’sine göre yorumlanır. Örn., `http://domain.example/icecream/chocolate.html` sayfasında:
`strawberry.html` → `http://domain.example/icecream/strawberry.html`

Wikipedia: URI Resolution

---

## ✍️ Zengin Metin (RichText)

Kalın, italik, köprü vb. dâhil zengin içerik düzenlemeyi etkinleştiren ortak bileşen.

---

## 📰 RSS (RSS)

**“Really Simple Syndication”**: Blog girdileri, torrent dosyaları, haber benzeri sitelerdeki video klipler gibi birçok içerik türünün yayılımı için kullanılan biçimdir; özellikle sık güncellenen içerikler için kullanılır ve bir tür “feed” veya “aggregator” olarak da bilinir. Bir RSS beslemesi özet veya tam metin içerebilir ve insanların sevdikleri siteleri e-posta benzeri otomatik bir şekilde takip etmelerini kolaylaştırır.

Besleğin içeriği, **RSS/Feed reader** adı verilen yazılımlar ile okunur. Feed okuyucular; köprüleri (hyperlinks) görüntüler ve daha fazlasını okuyup okumamaya karar vermeye yardımcı olan diğer üstverileri (metadata) içerir.

RSS’in ilk amacı, bilgiyi sizin aramanız yerine (Web üzerinden), bilginin **size gelmesini** (feed reader aracılığıyla) sağlamaktır.

**News aggregator** adı verilen programlar, kullanıcıların çok sayıda beslemeyi aynı anda görmesine ve sürekli “push” içerik almasına izin verir. WordPress’e RSS beslemeleri getirme hakkında Codex kaynakları için **Category\:Feeds** bölümüne bakın. Bkz. **RDF Site Summary**.

---

## ↔️ RTL (RTL)

Bir yazı sistemi, yazı yönü sayfanın sağından soluna akıyorsa **sağdan sola (Right-to-left)** kabul edilir.

İlgili makaleler: Right-to-Left Language Support

---

## 🤖 Robots.txt (Robots.txt)

**Web Robotları**, Web’i otomatik olarak tarayan programlardır; **Web Wanderers**, **Web Crawlers** ve **Spiders** olarak da adlandırılır. Arama motorları başlıca Web Robotlarıdır. Bazı Web Robotları, sunucunuzda **robots.txt** adlı bir dosya arayarak sunucunuzdaki içerik ve dosyaları nerede ve nasıl arayacaklarını belirler; bazıları ise bu dosyayı yok sayar.

İlgili makaleler: Search Engine Optimization for WordPress
Dış bağlantılar: Google information about robots.txt, The Web Robots Page

---

## 👥 Rol (Role)

**Rol (role)**, kullanıcılara bir grup görevi gerçekleştirme izni verir. Bir kullanıcı oturum açıp kimliği doğrulandığında, kullanıcının rolü, sahip olduğu **yetkinlikleri (capabilities)** belirler; her yetkinlik, bir veya daha fazla görev türünü gerçekleştirme iznidir. Aynı role sahip tüm kullanıcılar normalde aynı yetkinliklere sahiptir. Örneğin, **Author** rolüne sahip kullanıcılar genellikle kendi yazılarını düzenleme iznine sahiptir; ancak diğer kullanıcıların yazılarını düzenleme iznine sahip değildir. WordPress’in rol tabanlı erişim sisteminde altı rol ve elliden fazla yetkinlik bulunur. Eklentiler sistemde değişiklik yapabilir.

İlgili makale: Roles and Capabilities
Dış bağlantı: Role-based access control – Wikipedia

---

## 🖼️ Ekran (Screen)

WordPress’te **ekran (screen)**, bir blogun (site) veya ağın belirli bir bölümünü yönetmek için kullanılan web sayfasıdır. “Page” WordPress’te farklı ve belirli bir anlama sahip olduğundan karışıklığı önlemek için “screen” terimi kullanılır. Örneğin, yazıları yönetmek için kullanılan web sayfası **Posts Screen** olarak bilinir.

İlgili makale: Class\_Reference/WP\_Screen

---

## 🔄 Serileştirme (Serialization)

Bir bloğun **öznitelikler nesnesini**, her blok düzenlendiğinde gerçekleşen bir süreçle **HTML işaretlemesine** dönüştürme işlemidir.

---

## 🧭 Ayarlar Kenar Çubuğu (Settings Sidebar)

Sağ tarafta, belge ve blok ayarlarını içeren paneldir. **Settings** dişli simgesi ile açılıp kapatılır. Bir blok seçiliyse blok ayarları; değilse belge ayarları gösterilir.

---

## 🖥️ Kabuk (Shell)

**Shell**, MS-DOS, Unix/Linux, Mac OS X vb. bir işletim sistemiyle doğrudan etkileşime giren programdır — en çok **Unix benzerleri** ile ilişkilendirilir. Fare veya grafik arayüz yerine yazılı komutlarla kontrol edildiğinden sıklıkla “konsol” veya “komut satırı” olarak anılır.

Uzak bir bilgisayarla etkileşim kurarken (ör. WordPress yapılandırırken) genellikle **SSH** adı verilen ek bir “sahte” shell devreye girer.

Yaygın shell programları:

* Bash (Bourne Again Shell)
* Tcsh (genişletilmiş bir C Shell)
* Zsh

---

## 🧩 Kısa Kod (Shortcode)

**Shortcode**, bir sayfanın veya diğer içerik ögesinin gövdesine küçük bir PHP kod parçası gömmek için kullanılan tekniktir.

---

## 🧱 Kenar Çubuğu (Sidebar)

**Kenar çubuğu (sidebar)**, web sayfasının ana içeriği dışında bilgi göstermek için bir temanın sağladığı dikey sütundur. Temalar genellikle içeriğin solunda veya sağında en az bir kenar çubuğu sağlar. Kenar çubukları, site yöneticisinin özelleştirebileceği **bileşenler (widgets)** içerir.

Bir temada kenar çubukları, genellikle `sidebar.php` adlı şablon dosyası tarafından oluşturulur.

Bkz.: Footer area
İlgili makaleler: Sidebars, Templates, Customizing Your Sidebar, Stepping Into Templates, Template Hierarchy

---

## 🌐 Site (Site)

WordPress kullanıcı arayüzünde **site**, WordPress tarafından oluşturulan web sitesi olabilir veya çoklu site özelliği kapsamında bir ağın parçası olarak oluşturulan **sanal bir web sitesi** olabilir. Ağdaki bir site, sunucuda kendi dizinine sahip olmaması anlamında sanaldır; ancak kendi URL’si ve hatta kendi alan adına sahip olabilir.

WordPress kodunda **site**, WordPress tarafından oluşturulan web sitesidir. **Multisite** kullanılıyorsa, **site** ağ web sitesini; her sanal web sitesi ise **blog**’u ifade eder.

İlgili makale: Create A Network

---

## 🛠️ Site Düzenleyici (Site Editor)

Çeşitli şablonlar, şablon parçaları, stil seçenekleri ve daha fazlası arasında doğrudan düzenleme ve gezinme olanağı sağlayan bütünleşik deneyimdir.

---

## 🏷️ Slug (Slug)

**Slug**, bir yazı veya sayfayı tanımlayan birkaç kelimedir. Genellikle WordPress tarafından otomatik oluşturulan **yazı başlığının URL dostu sürümüdür**; ancak slug istediğiniz herhangi bir şey olabilir. Slug’lar, URL’deki içeriği betimlemeye yardımcı oldukları için **kalıcı bağlantılarla (permalinks)** birlikte kullanılmak üzere tasarlanmıştır.

Örnek yazı kalıcı bağlantısı: `https://wordpress.org/development/2006/06/wordpress-203/`
Bu yazının **slug**’ı: `wordpress-203`.

Slug’lar, yazı türleri, kategoriler, etiketler vb. için de kullanılır; yazı ve sayfa slug’larında olduğu gibi, bu ögelerin URL dostu sürümlerini oluşturmak içindir.

---

## 🙂 İfadeler (Smileys)

**Smileys (Smilies veya Emoticons)**, genellikle iki nokta biçiminde gözler ve yarım ağızla sarı düğmeler olarak gösterilen, insan yüzünün stilize temsilleridir. WordPress Eklentilerinde sıkça kullanılır. Varsayılan olarak WordPress, metin ifadelerini otomatik olarak grafik görsellere dönüştürür. Yazınızda `😉` yazdığınızda, yazıyı önizlediğinizde veya yayımladığınızda görsel olarak görünür.

İlgili makale: Using Smilies

---

## 🚫 Spam (Spam)

Bir zamanlar **SPAM**, konserve bir hayvansal yan üründü ve pek çok Monty Python skeçlerinin konusu olmuştu; ancak internetin günlük yaşamın ayrılmaz bir parçası hâline gelmesiyle **Spam**, internetin sorunlarıyla eşanlamlı hâle geldi. Genel terimle **spam**, e-posta veya diğer istenmeyen reklam biçimleridir. İnternet boyunca çok kolay yayılır ve binlerce, hatta yüz binlerce istenmeyen reklam, dolandırıcılık veya şüpheli para kazanma yöntemlerini göndererek, çok küçük bir yüzdelik dilimin kandırılması hâlinde bile çok para kazanılabileceği prensibiyle çalışır.

Günümüzde yaygın spam, çevrimiçi kumar sitelerinden ve “erkeklik artırma” ilaçlarını satmaya çalışanlardan gelir. Son zamanlarda bloglar (web logs), arama motorlarındaki site puanlarını artırmak amacıyla spam’cilerin hedefi hâline gelmiştir. Spam’ciler, elektronik gereksiz postaları dağıtmak için çeşitli yöntemler kullanır; milyonlarca adres ve IP’ye hızla ve kolayca e-posta veya yorum göndermek için botlardan (bilgisayar programları) yararlanırlar.

Spam’cileri izlemek zor olabilir; çünkü genellikle insanların e-posta ve IP adreslerini ele geçirirler. Bu olduğunda, size spam’i bir arkadaşınız göndermiş gibi görünebilir; oysa spam’cinin botu arkadaşınızın e-posta adresini yakalamış ve gerçek kaynağı gizlemek için kullanmıştır. WordPress geliştiricileri ve topluluk üyeleri, interneti çöpleriyle tıkayan bu rahatsız edici spam’cilerle mücadele için sürekli daha iyi yöntemler üzerinde çalışmaktadır. Siz de yeteneklerinizi, fikirlerinizi, önerilerinizi sunarak veya dikkatli davranıp mevcut spam karşıtı araçları kurarak yardımcı olabilirsiniz.

Dış bağlantılar: SPAM – Wikipedia


## 🔐 Güvenli Kabuk (SSH – Secure Shell)

SSH, TCP/IP üzerinden uzak bilgisayarlara bağlanmak için kullanılan bir iletişim protokolüdür. Çeşitli kimlik doğrulama yöntemleri kullanılabildiğinden, SSH **Telnet**’ten daha güvenlidir.

---

## 🔒 Güvenli Yuva Katmanı (SSL – Secure Sockets Layer)

SSL, **Taşıma Katmanı Güvenliği (TLS – Transport Layer Security)**’nin öncüsüdür. İnternet gibi güvensiz ağlar üzerinden güvenli iletişim için kullanılan kriptografik protokollerdir.

Dış bağlantılar: SSL at Wikipedia

---

## 🧱 Statik blok (Static block)

İçeriği bir yazı kaydedilirken bilinen blok türüdür. Statik bir blok, HTML işaretlemesiyle doğrudan yazı içeriğine kaydedilir.

---

## 📈 İstatistikler (Stats)

Belirli bir zaman aralığında bir WordPress blogu veya web sitesinin aldığı görüntüleme ve ziyaretçi sayısını gösteren kayıtlardır. İstatistikler ayrıca ziyaretçilerinizin dünyadaki konumlarını da gösterir.

---

## 🔤 Dize (String)

Bilgisayar biliminde **string (dize)**, sonlu sayıda karakterden (harfler, rakamlar, semboller ve noktalama işaretleri) oluşan herhangi bir dizidir. Verinin sayı ya da değişken adı değil de dize olarak tanınması için genellikle tırnak işaretleri içinde yazılması gerekir.

Dış bağlantılar: String at Wikipedia

---

## 🏗️ Yapı etiketleri (Structure tags)

WordPress kalıcı bağlantılarını (permalinks) özelleştirmek için kullanılan etiketlerdir: `%year%`, `%day%`, `%hour%`, `%minute%`, `%second%`, `%post_id%`, `%postname%`, `%category%` ve `%author%`. Her kalıcı bağlantının tek bir yazıya işaret etmesi için yapıyı `%post_id%` veya `%postname%` ile bitirin.

İlgili makaleler: Permalinks

---

## 🗂️ Subversion (Subversion)

Subversion, WordPress Geliştiricileri tarafından çeşitli WordPress sürümlerindeki değişiklik ve güncellemeleri izlemek için kullanılan açık kaynaklı bir sürüm kontrol yazılımıdır.

İlgili makaleler: Using Subversion
Dış bağlantılar: Subversion access at wordpress.org, Subversion book at red-bean.com

---

## 🔌 SVC (SVC – Switched Virtual Circuit)

SVC, bir **anahtarlamalı sanal devredir (Switched Virtual Circuit)** ve veri aktarım oturumu süresince geçici olarak devreye alınır.

Dış bağlantılar: Virtual circuit at Wikipedia

---

## 🔁 Yayınlama (Syndication)

Bkz.: **RSS – Really Simple Syndication**

---

## 🏷️ Etiket (Tag)

**Etiket (tag)**, bir Yazıyı (Post) tümüyle ya da kısmen tanımlayan anahtar kelimedir. Kategoriye benzer ancak kapsamı daha dardır. Bir yazıda, yazıyla yalnızca kısmen ilişkili olabilecek birden fazla etiket bulunabilir. Kategoriler gibi Etiketler de genellikle aynı etikete sahip tüm yazıları gösteren bir sayfaya bağlanır. Etiketler, Etiket alanına yazarak anında oluşturulabilir. Varsayılan olarak etiketler yalnızca Yazı ve özel yazı türlerine atanabilir.

Etiketler, çok sayıda etiketi farklı boyut ve renklerle gösteren **bulutlar (tag clouds)** hâlinde de sunulabilir; bu, blogunuzun genel konularını görselleştirir.

Birçok kişi Etiket ve Kategoriyi karıştırır; fark şudur: Kategoriler genellikle sık değişmezken, Etiketler yazıya daha yakındır ve her yazıyla birlikte değişebilir.

---

## ✍️ Slogan (Tagline)

**Slogan (tagline)**, blogun karakterini veya niteliklerini kısa ve öz biçimde tanımlayan akılda kalıcı ifadedir. Bir web günlüğü için “slogan” olarak düşünebilirsiniz.

---

## 🧭 Görev Tabanlı Dokümantasyon (Task Based Documentation)

**Görev tabanlı (task oriented)** dokümantasyon, sizi bir süreci/adımı adım adım ilerleten yazımdır; özlüdür, jargon içermez, kolay anlaşılır ve tamamen belirli görevleri gerçekleştirmeye odaklanmıştır. Z’ye ulaşmak için şunları yapmanız gerekir:

* Adım x
* Adım y
* Adım z

Unutmayın: Bir görevi nasıl yapacağını öğrenmek isteyen kişiler genellikle hızlı yanıta ihtiyaç duyar!

---

## 🧮 Taksonomi (Taxonomy)

**Taksonomi (taxonomy)**, şeylerin sınıflandırılmasını sağlar. WordPress’te iki yerleşik taksonomi vardır: **kategoriler (categories)** ve **etiketler (tags)**. Bu taksonomiler, yazıları ve özel yazı türlerini daha ayrıntılı sınıflandırır. Ayrıca, **özel taksonomiler (custom taxonomies)** de tanımlanabilir.

Bkz.: Category, Tag
Dış bağlantılar: Taxonomy at Wikipedia, `register_taxonomy()`

---

## 🖥️ Telnet (Telnet)

Telnet, başka bir bilgisayara bağlantı kurmak için kullanılan bir iletişim protokolüdür. TCP/IP üzerinde çalışır ve genellikle terminal öykünme yazılımlarıyla birlikte uzak bilgisayarlara oturum açmak için kullanılır. **Telnet özünde güvensizdir** ve büyük ölçüde **SSH** ile değiştirilmiştir.

Dış bağlantılar: Telnet at Wikipedia

---

## 🧩 Şablon (Template)

WordPress’te **şablon (template)**, bir temanın oluşturduğu web sayfalarının belirli bir alanını tanımlayan dosyadır. Örneğin, sayfaların üst kısmındaki **üstbilgi (header)** için bir şablon, içerik için bir şablon, kenar çubukları (sidebars) için bir şablon vb. bulunur. Şablonlar, tüm web sayfasını oluşturan yapı taşları gibidir.

İlgili makaleler: Templates, Stepping Into Templates, Template Hierarchy

---

## 📝 Şablon Düzenleme Modu (Template Editing Mode)

Bir yazı/sayfanın kullandığı şablonu düzenlemenize/değiştirmenize/oluşturmanıza olanak tanıyan, ölçeklendirilmiş doğrudan düzenleme deneyimi.

---

## 🔖 Şablon Etiketi (Template Tag)

Bir WordPress Temasında, **şablon etiketleri (template tags)**, şablon dosyalarında belirli programlama talimatları üretmek için kullanılır. Bir WordPress sitesinde oluşturulan içerik ve bilgileri görüntülemek için kullanılırlar. **Template tags**, WordPress çekirdeğine talimatlar için bağlanan kısa programlama sözcükleridir (fonksiyonlardır). Örneğin, bir WordPress sitesinin HTML `title` etiketi, site başlığını, site sloganını ve diğer site bilgilerini parametrelerine göre isteyen `bloginfo()` şablon etiketini içerebilir. Bu yaklaşım, Temanın farklı sitelerde kullanılmasına olanak tanır; böylece görüntülenen bilgiler siteye göre kolayca değişir.

Diğer şablon etiketleri daha karmaşıktır; yazı içeriği, sorgular ve site verileri üretir.

İlgili makaleler: Stepping Into Template Tags, Anatomy of a Template Tag, How to Pass Tag Parameters, Include Tags, Conditional Tags, Function Reference, Templates

---

## 🏷️ Terim (Term)

WordPress’te **terim (term)**, bir **Taksonomi (Taxonomy)** içindeki sınıflandırma, grup veya alt kümeyi ifade eder; taksonomi bir **Kategori (Category)**, **Etiket (Tag)** veya **Özel Taksonomi (Custom Taxonomy)** olabilir. Varsayılan olarak terimlerin bir **başlığı (title)**, **kısaltması (slug)** ve **açıklaması (description)** vardır. Kategoriler gibi hiyerarşik taksonomilerde, bir **üst terim (parent term)** tanımlanabilir.

İlgili makaleler: Taxonomies, `the_terms()`

---

## ✏️ Metin düzenleyici (Text editor)

**Metin düzenleyici (text editor)**, dosyaları **düz metin (plain text)** biçiminde düzenleyen programdır (ikili – binary biçime karşı). Düz metin temelli olmayan kelime işlemcileri (örn. Microsoft Word ile PHP betiklerini düzenlemek) kodunuzda ciddi sorunlara neden olabilir; çünkü bu programlar metin dosyalarına ekstra biçimlendirme ekler ve yorumlayıcı tarafından çalıştırılması gereken dosyaları bozabilir. **Not Defteri (Notepad)** gibi bir düzenleyici ekstra biçimlendirme eklemez.

WordPress dosyalarını yalnızca metin düzenleyiciyle düzenleyin.

Düz metin olarak düzenlenmesi gereken bazı dosya biçimleri:

* HTML belgeleri
* PHP betikleri
* Perl betikleri
* RTF (Rich Text Format) belgeleri
* JavaScript betikleri

Önerilen Metin Düzenleyiciler için **Editing Files** sayfasına bakınız.

Düz metin olmayan ve düzenleme için özel yazılım gerektiren örnek biçimler:

* Microsoft Word belgeleri
* Microsoft Excel hesap tabloları
* JPEG, PNG, GIF gibi görseller

Metin düzenleyebilen fakat temel metin düzenleyici sayılmayan ve WordPress dosyaları üzerinde **önerilmeyen** bazı yazılımlar:

* Microsoft Word
* Microsoft Excel
* Adobe Photoshop
* Adobe Illustrator
* Adobe Dreamweaver

---

## 🎨 Tema (Theme)

**Tema (Theme)**, bir site için grafiksel ön yüz arayüzünü ve altında birleşik bir tasarımı üreten dosyalar bütünüdür. WordPress Teması, WordPress’in çekirdek programlamasını değiştirmeden sitenin görüntülenme şeklini ve tasarımını değiştirir. Bazıları “siteyi giydirme (skinning)” ile özdeşleştirse de, bir WordPress Teması; PHP, WordPress şablon etiketleri, WordPress koşullu etiketleri ve CSS ile her sayfa görüntülemesinde tasarımı etkileyen programlama kodu içerir.

İlgili makaleler: Theme Development, Using Themes

---

## 🧱 Tema Blokları (Theme Blocks)

Geleneksel şablonlarda **template tags** ile mümkün olan her şeyi gerçekleştiren bloklardır (ör. **Post Author Block**). Tam liste için ilgili kaynağa bakınız.

---

## ✍️ TinyMCE (TinyMCE)

**TinyMCE**, web tabanlı bir JavaScript **WYSIWYG (What You See Is What You Get)** editörüdür.

---

## 🧰 Araç Çubuğu (Toolbar)

**Araç Çubuğu (Toolbar)**, sitenin hemen üstünde yer alan ve “yeni yazı ekle” veya “profilini düzenle” gibi yararlı yönetim ekranı bağlantılarını listeleyen alandır. Sürüm 3.1’de **Admin Bar** olarak eklendi, 3.3’te **Toolbar** ile değiştirildi. **User Profile Screen** üzerinden açılıp kapatılabilir.

İlgili makaleler: Toolbar
Bkz.: Admin Bar, Your Profile Screen

---

## 🧰 Araç Çubuğu (FSE’de) (Toolbar (in FSE))

Bir dizi düğme kontrolü. Blok bağlamında, genellikle seçili bloğun üstünde görünen blok kontrol araç çubuğunu ifade eder.

---

## 🔗 Geri İzleme (Trackback)

**Trackback**, doğrudan bir bağlantınız olmasa bile, başka bir yazarın blogunda yazdığı konuyla ilgili bir şey yazdığınızda onu haberdar etmenize yardımcı olur. Pingback ve trackback ile bloglar birbirine bağlanır. Bunu, akademik bir makalenin sonunda yer alan teşekkür ve kaynakça bölümlerinin bir karşılığı gibi düşünebilirsiniz.

Bkz.: Pingback
İlgili makaleler: Introduction to Blogging: Trackbacks

---

## ⏱️ Geçici veri (Transient)

**Transient**, hızlı erişim için web sunucusu veritabanında veya belleğinde, özel bir adla saklanan **geçici veridir**. Bu geçicilik ve hızlı bellek önbelleklemesi kullanımı, onları **Seçenekler (Options)**’dan ayıran temel özelliktir.

İlgili makaleler: Transients API, Options API

---

## 🌐 Unicode (Unicode)

Geniş ölçüde desteklenen ve tercih edilen bir **karakter kodlama sistemi (character encoding)**.

Bir bilgisayarın harfleri (veya herhangi bir karakteri) görüntüleyebilmesi için onları numaralandırması, yani bildiği karakterler için bir dizin oluşturması gerekir; bunlar **karakter kümeleri (character sets)** olarak bilinir. İngilizce dışındaki dillerde WordPress barındıran kullanıcılar için bu hayati önem taşır.

En yaygın karakter seti koleksiyonları **iso-8859**’dur; **iso-8859-1** ve **iso-8859-15** (euro işaretini içerir) en yaygın olanlarıdır; **Latin1** ve **Latin9** olarak da bilinirler. Bu kümeler, her karakter için 8 bit (bir bayt) kullanır ve 255 farklı karaktere izin verir (boş karakterle 256). Ancak Latin dilleri dışındaki diller (Japonca veya İbranice gibi) düşünüldüğünde 255 karakter yeterli değildir.

**Unicode**, çok geniş bir karakter dizinidir. Öyle ki bazen karakterleri temsil etmek için 16 bitten (2 bayt) fazlası gerekir. Ayrıca Unicode’un ilk 127 karakteri, en yaygın karakter kümesi olan **iso-8859-1**’in ilk 127 karakteriyle aynıdır. Bu amaçla **UTF (Unicode Translation Format)** oluşturulmuştur. UTF, karakterler için değişken bit sayıları kullanır ve Unicode’un tüm aralığının kullanılmasına izin verir. Bilmeniz gerekenler:

* **UTF-8**, UTF’nin en az 8 bit kullanan türüdür. **UTF-16** ve **UTF-32** de vardır.
* Belgeniz Latin tabanlı bir kodlamadaysa, onu UTF yapmak için muhtemelen hiçbir şey değiştirmeniz gerekmez.
* Tek bir UTF belge, kodlama değiştirmeden çeşitli dillerde olabilir.

Dış bağlantılar: Joel Spolsky on Unicode

---

## 🖥️ Unix (Unix)

**Unix (UNIX)**, 1969’dan itibaren AT\&T’nin Bell Laboratuvarlarında geliştirilen bir işletim sistemidir. Başlangıçta assembly yerine **yüksek seviyeli bir dil** ile yazılmış bir işletim sistemi oluşturma hedefiyle tasarlanmıştır. Günümüzde web sunucularının çoğu, bu yüksek performanslı işletim sisteminin farklı “çeşitleri” üzerinde veya Unix benzeri bir işletim sistemi olarak geliştirilen **Linux** üzerinde çalışır.

Bkz.: UNIX Shell Skills, Mac OS X

---

## ⏰ Unix Zamanı (Unix Time)

**Unix Time (timestamp)**, belirli bir olaydan (Epoch) bu yana geçen yaklaşık saniye sayısını belirleyerek zamanı izleme yöntemidir. Yüzyılda yalnızca birkaç saniyelik sapma olduğundan çoğu uygulama için yeterince doğrudur.

Unix zamanı (günümüzde) on haneli bir sayıdır, örn. `1229362315`. WordPress, zamanı izlemek için dahili olarak sıklıkla Unix zaman damgasını kullanır. Okunabilir tarih ve saatler, Unix Zamanı’ndan veya MySQL/MariaDB **DATETIME** alanından dönüştürülür.

Dış bağlantılar: Unix Time at Wikipedia, DATETIME, MariaDB DATETIME

---

## 🔗 URL (URL)

İnternette belirli bir web sitesi veya dosyanın adresidir.

```
http://www.example.com/
http://www.example.com/reports/index.html
```

---

## 🌍 UTC (UTC – Universal Time, Coordinated)

**UTC**, dünya çapındaki saat dilimlerinin hesaplandığı uluslararası zaman standartlarının temelidir. Çoğu amaç için eski **GMT** standardıyla aynıdır.

Dış bağlantı: UTC (Wikipedia)

---

## 🖧 Web sunucusu (Web server)

**Web sunucusu (web server)**, HTML ile yazılmış web sitelerini barındırmak/sunmak için yazılıma ve altyapıya sahip bilgisayardır. İnternette en yaygın web sunucusu yazılımı **Apache**’dir ve sıklıkla **PHP**, **Perl** ve diğer betik dilleriyle birlikte kullanılır.

Her hızdaki internet bağlantısı üzerinde kendi web sunucunuzu kurmak mümkündür; ancak çoğu kişi, sık ziyaret edilen siteler için yeterli bant genişliği, çalışma süresi, donanım ve bakım sunabilen **barındırma sağlayıcılarından** paket satın almayı tercih eder.

İlgili makaleler: Hosting WordPress

---

## 🧱 Bileşen (Widget)

WordPress’te **widget**, bir web sayfasında belirli bir işlevi yerine getiren kendi kendine yeterli alan ya da bunu üreten koddur. Örneğin, WordPress’te bir kenar çubuğunda (sidebar) sayfa listesini gösteren yerleşik bir widget ve Gösterge Paneli’nde (Dashboard) son yorumları gösteren başka bir yerleşik widget bulunur. Eklentiler ve temalar ek widget’lar sağlayabilir.

İlgili makaleler: WordPress Widgets, Widgets API, Dashboard Widgets API

---

## 🧱 Bileşen Alanı (Widget Area)

**Widget Area**, bir WordPress Temasının kodunda, kullanıcıların Widget’ları yerleştirmesine izin veren, önceden tanımlı bir konumdur.

---

## 🤝 XFN (XFN – XHTML Friends Network)

**XFN**, bloglar arası bağlantıların blog yazarları arasındaki ilişkileri temsil ettiği, merkezi olmayan bir projedir. XFN bağlantıları şu biçimde olabilir:
`<a href="http://www.photomatt.net/" rel="friend met">Photo Matt</a>`

---

## 🧾 XHTML (XHTML – Extensible HyperText Markup Language)

**XHTML**, tüm web sayfalarının oluşturulduğu W3C standart dili olarak **HTML**’in halefidir. Genellikle **CSS** ve **JavaScript** ile birlikte kullanılır.

WordPress, **XHTML 1.0 Transitional** standardına uymaya çalışır.

Dış bağlantılar: XHTML 1.0 Specification (Second Edition), XHTML 1.1 Specification

---

## 📦 XML (XML – Extensible Markup Language)

**XML**, **SGML (Standard Generalized Markup Language)** üzerinde yazılmıştır ve özünde kendi işaretleme dilinizi tanımlamanıza olanak tanır. İnternet genelinde verileri tanımlamak, paylaşmak ve iletmek için son derece kullanışlıdır. Genellikle **HTML** ile birlikte kullanılır; **XML** veriyi tanımlar, **HTML** bu veriyi görüntüler.

Dış bağlantılar: Extensible Markup Language (XML) Resources at W3C org, XML 4.0 FAQ, Overview of SGML Resources at W3C org

---

## 🔌 XML-RPC (XML-RPC – Extensible Markup Language-Remote Procedure Call)

**XML-RPC**, bir **Uzak Prosedür Çağrısı (RPC – Remote Procedure Call)**’nın XML ile biçimlendirilmiş isteklerle başka bir uygulamaya gönderilmesini sağlar ve o uygulamanın bu isteği yerine getirmesini bekler. Yani kullanıcı (veya geliştirici), XML olarak biçimlendirilmiş bir isteği harici bir uygulamaya gönderebilir.

İlgili makaleler: XML-RPC Support
Dış bağlantılar: Dave Winer’s XML-RPC for Newbies, XML-RPC Home Page, Apache XML-RPC, XML-RPC for PHP Homepage, XML-RPC at Wikipedia

---

## 📚 Daha Fazla Kaynak (More Resources)

Blog terimleri, kısaltmalar ve kısmi sözlükler:

* Giant Blogging Terms Glossary
* Blogging Terms at Wikipedia
* External WordPress glossary with additional terms

---

## 🗂️ Kategoriler (Categories)

* WordPress Help
* Troubleshooting
* Getting Started
* Advanced Topics
* UI Link

Back to the Top

---

