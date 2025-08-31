# WordPress Semantics

## 📝 WordPress Anlambilimi (semantics)

### 📖 Terminolojiye giriş (terminology introduction)

Geliştiriciler WordPress’i bir weblogging (blog yazarlığı) sistemi olarak oluşturdu. Codex Sözlüğü’nde tanımlandığı gibi bir blog, “bir kişi ya da grup tarafından yayınlanan çevrimiçi bir günlük, hatıra defteri veya dizi”dir. Birçok blog kişisel nitelikte olup, sahibinin görüşlerini ve ilgi alanlarını yansıtır. Ancak günümüzde bloglar haber, iş dünyası, siyaset ve eğlence dünyasında önemli araçlar haline gelmiştir.

Bloglar, Wikipedia’nın “işbirliğine dayalı içerik oluşturmayı düzenlemek ve kolaylaştırmak için kullanılan bir sistem” olarak tanımladığı İçerik Yönetim Sistemi (Content Management System – CMS) türüdür. Hem bloglar hem de İçerik Yönetim Sistemleri bir web sitesinin (kısaca site) rolünü üstlenebilir. Bir web sitesi, belirli bir konu, hizmet veya ürün hakkında makale ve bilgilerin bir araya geldiği bir koleksiyon olarak düşünülebilir; bu, sahibinin kişisel yansıması olmak zorunda değildir. Son zamanlarda WordPress’in rolü genişledikçe, WordPress geliştiricileri blog yerine daha genel bir terim olan site kelimesini kullanmaya başlamışlardır.

### 📚 İçerik terminolojisi (content terminology)

WordPress’teki Word (kelime) terimi, yazıları (post) oluşturmak için kullanılan kelimelere karşılık gelir. Yazılar (postlar), bir blogun ana unsurunu (ya da içeriğini) oluşturur. Yazılar, blog sahibinin veya misafir yazarların yazıları, kompozisyonları, tartışmaları, söylemleri, düşünceleri ve hatta çıkışmalarıdır. Çoğu durumda yazılar, bir blogun var olma sebebidir; yazılar olmadan blog da olmaz!

Bir blogun ayrılmaz parçaları resimler, görseller, sesler ve filmler olup bunlara medya (media) denir. Medya, bir blogun içeriğini zenginleştirir ve ona hayat verir. WordPress, Medya’yı doğrudan yazılara eklemek, daha sonra yazılara iliştirilebilecek şekilde yüklemek ve tüm Medya’yı yönetmek için bir Medya Kütüphanesi (Media Library) sunar.

Yazı sürecinin önemli bir parçası, bu yazıları kategorilere (categories) atamaktır. WordPress’te her yazı bir veya daha fazla kategori altında dosyalanır. Kategoriler hiyerarşik olabilir; bir kategori, birkaç alt veya torun kategoriye ebeveynlik edebilir. Düşünülerek yapılan kategorizasyon, benzer içerikteki yazıların gruplandırılmasını sağlayarak siteyi ziyaret edenlerin gezinmesine ve kullanmasına yardımcı olur. Kategorilere ek olarak, her yazıya etiket (tag) adı verilen terimler veya anahtar kelimeler atanabilir. Etiketler bir başka gezinme aracı görevi görür, fakat hiyerarşik değildir. Hem kategoriler hem de etiketler, taksonomiler (taxonomies) adı verilen bir sistemin parçasıdır. Kategoriler ve etiketler yetersiz kalırsa, kullanıcılar gönderiler, sayfalar veya özel yazı tipleri (custom post types) için daha özel tanımlamalar sağlayacak özel taksonomiler de oluşturabilir.

Bununla birlikte, yazı kategorileri ve etiketler yazı meta verisinin (post meta data) unsurlarından ikisidir. Yazı meta verisi, her yazıyla ilişkili bilgileri ifade eder ve yazarın adı, yazının tarihi ve kategorilerini içerir. Yazı meta verisi ayrıca özel alanlara (Custom Fields) da karşılık gelir; burada yazıları tanımlayabilecek özel kelimeler veya anahtarlar atanabilir. Ancak yazı meta verisinden söz ederken, meta teriminden de bahsetmek gerekir.

Genel olarak meta, “hakkında bilgi” anlamına gelir; WordPress’te meta genellikle yönetimsel türde bilgiyi ifade eder. Yazı meta verisine ek olarak, Meta dış dünyaya bir web sayfasını tanımlamak için kullanılan HTML etiketidir; örneğin arama motorları için meta etiket anahtar kelimeleri. Ayrıca birçok WordPress tabanlı sitede, genellikle kenar çubuğunda bulunan ve siteye giriş veya kayıt bağlantıları içeren bir Meta bölümü vardır. Ve tabii ki Meta Kuralları: Bu Codex’i kullanırken uyulacak genel protokolü tanımlayan kurallar ya da Codex içindeki yönetimsel işlevlere karşılık gelen MediaWiki ad alanı. Evet, oldukça fazla Meta var!

Bir yazı yayınlandığında, blogun okuyucuları yorumlar (comments) aracılığıyla bu yazıya yanıt verir ve yazarlar da karşılık verir. Yorumlar, yazar ve okuyucu arasındaki iletişim sürecini, yani karşılıklı etkileşimi sağlar. Yorumlar çoğu blogun can damarıdır.

Son olarak, WordPress iki başka içerik yönetim aracı daha sunar: Sayfalar (Pages) ve özel yazı tipleri (custom post types). Sayfalar genellikle “Hakkımda” veya “İletişim” gibi statik bilgileri sunar. Genellikle “zamansız” nitelikte olan Sayfalar, zaman odaklı nesneler olan yazılarla karıştırılmamalıdır. İlginçtir ki, bir Sayfa yorum alabilir fakat kategorilere ayrılamaz. Özel yazı tipi (custom post type), bir yazı veya sayfadan farklı yapılandırılmış veri türüdür. Özel yazı tipleri, kullanıcıların portföyler, projeler, video kütüphaneleri, podcastler, alıntılar, sohbetler ve kullanıcı veya geliştiricinin hayal edebileceği her şeyi kolayca oluşturup yönetmesini sağlar.

### 🎨 Tasarım terminolojisi (design terminology)

Bir WordPress Teması (Theme), bir sitenin genel tasarımı olup renk, grafik ve metni kapsar. Tema bazen skin (kaplama) veya template (şablon) olarak da adlandırılır, fakat gerçekte değildir. Skin ve template, esasen web sitesi için bir boya işidir. WordPress Teması ise kod ile tasarımın buluştuğu yerdir ve sitenin, yönetici tarafından belirlenen özel koşullara göre değişmesine izin verir.

WordPress Temalarının kurulumu, Yönetim Ekranlarındaki (Administration Screens) Temalar Menüsü ile kolaylaştırılmıştır. Resmi WordPress Tema Dizini’nden (Theme Directory) yeni bir Tema arayın ve birkaç tıklamayla etkinleştirin. Ayrıca kurmadan ve etkinleştirmeden önce temanızı önizleyerek sitenizin bu Tema ile nasıl görüneceğini görebilirsiniz.

WordPress’in esnekliği, bir WordPress sitesinin tasarımıyla ilgili terminoloji konuşulurken açıkça görülür. WordPress’in merkezinde, yazıları işlemek için The Loop adı verilen bir programlama yapısı vardır. The Loop, yazıları görüntülemek için kullanılan kritik PHP program kodudur. WordPress’i geliştirmek ve özelleştirmek isteyen herkesin The Loop’un işleyişini anlaması gerekir.

The Loop’un yanı sıra, WordPress geliştiricileri, tasarımcıların belirli eylemleri gerçekleştirmesine veya belirli bilgileri görüntülemesine olanak tanıyan PHP işlevlerinden oluşan Template Tags (şablon etiketleri) oluşturmuştur. Şablon etiketleri, Şablon Dosyalarının (Template Files) temelini oluşturur. Şablon dosyaları, bir WordPress sitesinin yapısını ve akışını kontrol eden şablon etiketleri gibi programlama parçalarını içerir. Bu dosyalar WordPress MySQL veritabanından bilgi alır ve web tarayıcısına gönderilen HTML kodunu üretir. Bir Şablon Hiyerarşisi (Template Hierarchy), yani işleme sırası, Şablonların çıktıların neredeyse tüm yönlerini nasıl kontrol ettiğini belirler; Başlıklar (Headers), Kenar Çubukları (Sidebars) ve Arşivler (Archives) gibi. Arşivler, genellikle tarih, kategori, etiket veya yazar bazında gruplandırılmış dinamik olarak üretilen yazı listeleridir.

WordPress’in yetenekleri geliştikçe, geliştiriciler kullanıcıların sitelerinin görünümünü ve işlevselliğini kolayca yönetmelerine olanak tanıyan araçlar eklemiştir:

* Bileşenler (Widgets), kenar çubuğuna mevcut hava durumu gibi küçük programlar eklemeyi kolaylaştırır.
* Menüler (Menus), genellikle bir sitenin sayfalarının üst kısmında bulunan gezinme düğmelerini tanımlamayı kolaylaştırır.
* Arka Plan aracı (Background tool), kullanıcının sitenin arka plan resmini ve rengini değiştirmesine izin verir.
* Başlık aracı (Header tool), kullanıcının sitenin farklı sayfalarının üst kısmında görüntülenen resimleri kontrol etmesini sağlar.
* Yazı Biçimleri (Post Formats), belirli bir yazının nasıl görüntüleneceğini kontrol etmeye olanak tanır (ör. bu yazıyı bir Aside, alıntı veya galeri olarak görüntüle).
* Eklentiler (Plugins), WordPress’in temel işlevselliğini genişletmek için oluşturulmuş özel işlevlerdir. WordPress geliştiricileri, dış geliştiricilere kendi faydalı eklenti özelliklerini oluşturma fırsatı vererek maksimum esneklik ve minimum kod şişkinliği sağlamıştır. WordPress Eklenti Dizini (Plugin Directory) bunun kanıtıdır; WordPress’in neredeyse her yönünü geliştirecek bir Eklenti mevcuttur.

Bir eklenti yönetim aracı, resmi dizinden eklentileri bulmayı ve yüklemeyi son derece kolay hale getirir.

### ⚙️ Yönetim terminolojisi (administrative terminology)

WordPress sitesinin Yönetimi (Administration) ile ilgili terimler bir başka inceleme konusudur. Kapsamlı bir Yönetim Ekranları (Administration Screens) seti, kullanıcıların bloglarını kolayca yönetmesini ve izlemesini sağlar. Bir WordPress yöneticisinin yetkileri arasında ziyaretçilerin bloga katılabilmesi için kayıt olma zorunluluğu getirme, kimlerin yeni yazı oluşturabileceği, yorum bırakılıp bırakılamayacağı ve bloga dosya yüklenip yüklenemeyeceği vardır.

Bir WordPress blog yöneticisinin ana sorumluluklarından bazıları Kayıtlı Kullanıcıların (Registered Users) eklenmesi, silinmesi ve yönetilmesidir. Kullanıcıları yönetmek, Roller (Roles) ve Yetkinlikleri (Capabilities), yani izinleri kontrol etmek anlamına gelir. Roller, kayıtlı bir kullanıcının hangi işlevleri gerçekleştirebileceğini belirler; bu işlevler sadece bloga giriş yapmaktan yönetici rolünü yerine getirmeye kadar değişebilir.

Blog yöneticisinin bir diğer önemli konusu ise Yorum Denetimi’dir (Comment Moderation). Yorumlar, yani tartışmalar, ziyaretçiler tarafından yazarlara bırakılan yanıtlar olup bir blogun “karşılıklı etkileşim”inin önemli bir parçasını oluşturur. Ancak yorumlar Spam ve diğer kötü niyetli amaçlar açısından denetlenmelidir. WordPress Yönetim Yorum Ekranı (Administration Comments Screen), yorumları ekleme, değiştirme ve silme işlemlerini kolaylaştırarak bu süreci basitleştirir.

Ve unutmamak gerekir ki, bir yöneticinin sorumluluğu WordPress’i güncel tutmaktır; böylece en yeni özellikler, hata düzeltmeleri ve güvenlik yamaları uygulanır. Yöneticiler için WordPress, en son sürümü indirmek ve yüklemek üzere basit bir Güncelleme Ekranı (Upgrade Screen) sağlar. Güncellememek için hiçbir bahane yok!

### 🆘 Yardım terminolojisi (help terminology)

Son jargon seti, WordPress konusunda size yardımcı olacak terimlerle ilgilidir. Her şeyden önce, her Yönetim Ekranının altında görünen Askıda Yardım sekmesi (Help tab) vardır. Bu bağlamsal yardım, mevcut ekranın işlevini ve kullanımını açıklar ve diğer yardım konularına bağlantılar sağlar. WordPress kullanıcıları için başka yardım kaynakları da mevcuttur; WordPress Yardımı Bulma (Finding WordPress Help), Sorun Giderme (Troubleshooting) ve WordPress SSS (FAQ – frequently asked questions) iyi başlangıç noktalarıdır. Ayrıca WordPress’e Başlarken (Getting Started with WordPress), okuyucuları WordPress dünyasına hızla dahil eder ve mükemmel WordPress Dersleri (WordPress Lessons), WordPress kullanmanın birçok yönü hakkında derinlemesine öğreticiler sunar. En önemli kaynaklardan biri WordPress Destek Forumu (Support Forum) olup bilgili gönüllüler sorularınızı yanıtlar ve WordPress ile ilgili sorunların çözümüne yardımcı olur. Ve tabii ki bu Destek sitesi (Support site), WordPress deneyiminizi başarılı kılmak için hazırlanmış yüzlerce makaleyle doludur!

### 📎 Daha fazla bilgi ve kaynaklar (more information and resources)

Ayrıca bakınız:

* WordPress Sözlüğü (Glossary)
* WordPress Özellikleri (Features)
* WordPress Destek Forumu (Support Forum)
