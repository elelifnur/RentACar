# RentACar
Bu proje, bir Araç Kiralama Yönetim Sistemi'dir. Sistem, kullanıcıların araç kiralamasına olanak tanırken, araç, marka, model ve kullanıcı yönetimini sağlar. Projede temel olarak üç ana katman bulunur: iş katmanı (business), veri erişim katmanı (DAO), ve kullanıcı arayüzü katmanı (view).

Katmanlar:
İş Katmanı (Business):

Bu katman, markalar, araçlar, modeller ve kullanıcılar gibi ana bileşenlerin iş mantığını yönetir.
Örneğin, BrandManager, araç markalarını yönetmek için CRUD (oluşturma, okuma, güncelleme, silme) işlemlerini sağlar. Benzer şekilde CarManager, UserManager ve ModelManager sınıfları, ilgili varlıkların yönetimini üstlenir.
Veri Erişim Katmanı (DAO):

Bu katman, veritabanı ile iş katmanı arasındaki köprüyü sağlar.
Her bir varlık (araba, marka, model, kullanıcı, rezervasyon) için ayrı DAO sınıfları bulunur. Bu sınıflar, veritabanına erişim işlemlerini gerçekleştirir ve iş katmanına veri sağlar.
Kullanıcı Arayüzü Katmanı (View):

Kullanıcılar, bu katman üzerinden sisteme erişir ve işlemlerini gerçekleştirir.
Örneğin, AdminView yöneticilerin markaları, modelleri, araçları ve rezervasyonları yönetmesine olanak tanırken, BookingView kullanıcıların araç kiralama işlemlerini yapmalarını sağlar.
Özellikler:
Araç Kiralama: Kullanıcılar, sistem üzerinden araç kiralama işlemlerini yapabilir ve uygunluk durumuna göre araç seçebilirler.
Yönetici Paneli: Yöneticiler, araç, model ve marka bilgilerini güncelleyebilir ve kiralama rezervasyonlarını takip edebilirler.
Veritabanı Yönetimi: DAO katmanı sayesinde araçlar, kullanıcılar ve rezervasyonlar gibi bilgiler veritabanında saklanır ve yönetilir.
Kullanıcı Doğrulama: Sistemde kullanıcı doğrulaması yapılabilir ve farklı kullanıcı rollerine göre yetkilendirme sağlanabilir (örneğin yönetici ve müşteri).
