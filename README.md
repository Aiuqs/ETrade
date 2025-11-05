# Proje: ETrade

Bu proje, .NET 7 kullanılarak geliştirilmiş bir E-Ticaret platformudur.

## 📝 Açıklama

Projenin amacı, (kullanıcıların ürünlere göz atması, sepete eklemesi, sipariş vermesi vb.) gibi temel e-ticaret işlevlerini sağlamaktır. Bu bölümde projenizin mimarisi (örneğin, Katmanlı Mimari, Onion Architecture vb.) ve temel özellikleri hakkında daha fazla detay verebilirsiniz.

## 🚀 Kullanılan Teknolojiler

Projenin geliştirilmesinde kullanılan temel teknolojiler:

* **Backend:** ASP.NET Core 7 (.NET 7)
* **Veritabanı:**  SQL Server
* **ORM:**  Entity Framework Core
* **Mimari:** Web API, MVC
* **Frontend:** Razor Pages

## 🔧 Kurulum ve Çalıştırma

Projeyi yerel makinenizde çalıştırmak için aşağıdaki adımları izleyin:

1.  Bu depoyu klonlayın:
    ```bash
    git clone [https://github.com/Aiuqs/ETrade.git](https://github.com/Aiuqs/ETrade.git)
    ```
2.  Proje dizinine gidin:
    ```bash
    cd ETrade
    ```
3.  Gerekli .NET paketlerini geri yükleyin:
    ```bash
    dotnet restore
    ```
4.  `Etrade.WebAPI/appsettings.json` (veya benzeri) dosyasındaki veritabanı bağlantı dizgisini (Connection String) kendi yerel ayarlarınıza göre güncelleyin.
5.  (Entity Framework Core kullanıyorsanız) Veritabanı göçlerini (migrations) uygulayın:
    ```bash
    dotnet ef database update --project Etrade.Infrastructure
    ```
6.  Web API projesini çalıştırın:
    ```bash
    dotnet run --project Etrade.WebAPI
    ```
7.  Uygulama varsayılan olarak `https://localhost:XXXX` ve `http://localhost:YYYY` adreslerinde çalışmaya başlayacaktır.


## 🤝 Katkıda Bulunma

Katkıda bulunmak isterseniz, lütfen bir "issue" açın veya "pull request" gönderin.

## 📄 Lisans

(Varsa) Bu proje MIT Lisansı altındadır.
