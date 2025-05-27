# Personel Kayıt Formu
Visiual Studio 2022 ile "C# Windows Forms (.Net FrameWork)" kullanılarak hazırlanmıştır.

Programın baştan sona anlatım ve yazım videosu müsait zamanda eklenecektir.

Şimdilik asıl kaynaktan yararlanabilirsiniz.
[Video Bağlantısı](https://www.youtube.com/watch?v=Fg4f9dHKoBY)

Aşağıdaki sql querry ile gerekli veritabanını oluşturabilirsiniz.

Bunun için SQL Server kurulu bir sisteme ve SSMS yani "SQL Server Management Studio" uygulamasına ihtiyacınız var.

SQL Server kurulumu için [BTK AKADEMİ: Uygulamalarla SQL Öğreniyorum](https://www.btkakademi.gov.tr/portal/course/uygulamalarla-sql-ogreniyorum-8249) bağlantısından "2. Kurulumlar"sekmesinde ki ilk bölümden "3.SQL Bağlantısı ve Veritabanı oluşturma" sekmesinin sonuna kadar izlendiği taktirde başarıyla tamamlayabilirsiniz.

    -- Veritabanı oluşturma
    create database PersonelVeriTabani;

    -- Veritabanını kullanma
    use PersonelVeriTabani;

    -- Tbl_Personel tablosunu oluşturma
    create table Tbl_Personel (
        PersonelId int primary key identity(1,1),
        PerAd nvarchar(max),
        PerSoyad nvarchar(max),
        PerSehir nvarchar(max),
        PerMaas int,
        PerDurum nvarchar(max),
        PerMeslek nvarchar(max)
    );
