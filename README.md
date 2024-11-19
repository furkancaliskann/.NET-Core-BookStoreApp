# .NET-Core-BookStoreApp

.NET Core Web API tabanlı bir Kitap Mağazası Uygulamasıdır. Bu projede, kitaplarla ilgili CRUD (Create, Read, Update, Delete) işlemleri, sayfalama, sıralama, filtreleme gibi gelişmiş özellikler sağlanmaktadır. Uygulama, Entity Framework Core (EF Core) ve Katmanlı Mimari prensiplerine göre geliştirilmiştir.

## Özellikler

- **Kitapları Listeleme**: Tüm kitapları listeleme işlevi sunar.
- **Kitap Güncelleme**: Kitap bilgilerini güncelleme özelliği.
- **Kısmi Güncelleme (PATCH)**: Kitap bilgilerini kısmi olarak güncelleme.
- **Kitap Silme**: Mevcut kitapları silme özelliği.
- **Kitap Getirme (ID'ye Bağlı)**: ID'ye göre kitap detaylarını getirme.
- **Sayfalama**: Büyük veri setleri için sayfalama desteği.
- **Sıralama**: Kitaplar üzerinde sıralama yapma.
- **Filtreleme**: Kitaplar üzerinde filtreleme işlemleri.
- **Loglama**: Uygulama içindeki kritik işlemler için loglama işlemleri.

## Teknolojiler

- **.NET Core Web API**: API geliştirme için kullanılan framework.
- **Entity Framework Core**: Veritabanı yönetimi ve ilişkili veritabanı işlemleri için kullanılan ORM.
- **Katmanlı Mimari**: Uygulama tasarımında katmanlı mimari kullanılmıştır.

## Kurulum

1. Bu projeyi kendi bilgisayarınıza klonlayın:

   ```bash
   git clone https://github.com/kullaniciadi/.NET-Core-BookStoreApp.git# .NET-Core-BookStoreApp


2. Proje klasörüne gidin:

    cd .NET-Core-BookStoreApp


3. Gerekli bağımlılıkları yükleyin:

    dotnet restore


4. Veritabanı bağlantısını appsettings.json dosyasındaki ConnectionStrings bölümüne uygun şekilde ayarlayın.


5. EF Core Migrations ile veritabanı oluşturun:

    dotnet ef database update


6. Uygulamayı başlatın:

    dotnet run

7. API'yi kullanmaya başlayabilirsiniz.



**API Endpoint'leri**

GET /api/books: Tüm kitapları listeleme.

GET /api/books/{id}: ID'ye göre kitap getirme.

POST /api/books: Yeni kitap ekleme.

PUT /api/books/{id}: Kitap bilgilerini güncelleme.

PATCH /api/books/{id}: Kitap bilgilerini kısmi güncelleme.

DELETE /api/books/{id}: Kitap silme.


**Geliştirici Notları**

Projede kullanılan veritabanı Entity Framework Core (EF Core) ile yönetilmektedir.
Veritabanı yapısı migrations kullanılarak oluşturulmuş ve güncellenmiştir.
Uygulama, Katmanlı Mimari kullanılarak yazılmıştır ve Service, Repository, Controller katmanlarına ayrılmıştır.
Kitap bilgileri, API üzerinde sayfalama, sıralama ve filtreleme özellikleriyle listelenebilir.


**Lisans**

Bu proje MIT Lisansı altında lisanslanmıştır. Detaylar için LICENSE dosyasına göz atabilirsiniz.