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
Aşağıdaki Querry ile örnek veriseti oluşturabilirsiniz.

    INSERT INTO Tbl_Personel (PerAd, PerSoyad, PerSehir, PerMaas, PerDurum, PerMeslek)
    VALUES 
        ('Ahmet', 'Yılmaz', 'İstanbul', 7500, '1', 'Mühendis'),
        ('Ayşe', 'Kara', 'Ankara', 6000, '0', 'Öğretmen'),
        ('Mehmet', 'Demir', 'İzmir', 5500, '1', 'Doktor'),
        ('Fatma', 'Çelik', 'Bursa', 8000, '0', 'Bankacı'),
        ('Ali', 'Şahin', 'Adana', 6500, '1', 'Eczacı'),
        ('Zeynep', 'Öztürk', 'Antalya', 5000, '0', 'Hemşire'),
        ('Murat', 'Koç', 'Konya', 7000, '1', 'Avukat'),
        ('Elif', 'Arslan', 'Trabzon', 5200, '0', 'Mimar'),
        ('Hasan', 'Turan', 'Eskişehir', 6800, '1', 'Yazılımcı'),
        ('Selin', 'Aydın', 'Mersin', 6200, '0', 'Psikolog');

Huzurlu bir kodlama dileğiyle...


