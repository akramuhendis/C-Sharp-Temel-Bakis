
# C# (C Sharp) Programlama Dili Hakkında Detaylı Bilgi

C# (C Sharp), Microsoft tarafından geliştirilmiş, modern, nesne yönelimli (OOP - Object-Oriented Programming) ve genel amaçlı bir programlama dilidir. C# dili, özellikle masaüstü, web ve mobil uygulamaları geliştirme için kullanılır. Ayrıca bulut tabanlı çözümler ve oyun geliştirme (Unity gibi oyun motorları) alanlarında da yaygın olarak tercih edilir.

## 1. C# Dilinin Temel Özellikleri
C# dili, güvenli ve verimli kod yazmayı hedefler. İşte dilin öne çıkan özellikleri:

### a. Nesne Yönelimli Programlama (OOP)
C# tam anlamıyla nesne yönelimli bir programlama dilidir. Bu, kodun daha iyi yapılandırılmasını sağlar. OOP'nin dört temel prensibi şunlardır:
- **Encapsulation (Kapsülleme):** Verilerin ve kodun gizlenmesi.
- **Abstraction (Soyutlama):** Gereksiz detaylardan arındırılmış bilgilerin gösterilmesi.
- **Inheritance (Kalıtım):** Sınıfların başka sınıflardan özellik ve metodlar miras alabilmesi.
- **Polymorphism (Çok Biçimlilik):** Aynı işlemin farklı biçimlerde uygulanabilmesi.

### b. Statik Tip Belirleme
C#, statik tip belirlemeli bir dildir. Bir değişkenin tipi derleme zamanında belirlenir ve değişmez.

### c. Güvenli ve Yönetilen Bellek
Bellek yönetimi, çöp toplama (Garbage Collection) mekanizması ile otomatikleştirilmiştir.

### d. Güçlü Tip Sistemi
Her değişkenin bir veri tipi vardır ve bu tipler katıdır. Veri türleri arasında dönüştürmeler açıkça yapılmalıdır (casting).

### e. Çoklu Platform Desteği
.NET Core ve .NET 5+ ile C#, Windows, macOS ve Linux üzerinde çalışabilir.

## 2. Temel Kavramlar ve Yapılar

### a. Değişkenler ve Veri Türleri
C# dilinde değişkenler bir veri türü ile tanımlanır. Yaygın kullanılan veri türleri şunlardır:

- **int:** Tamsayılar
- **double:** Ondalık sayılar
- **bool:** Doğru/yanlış
- **string:** Metin verileri
- **char:** Tek karakter
- **decimal:** Hassas ondalık sayılar

### b. Koşul İfadeleri (if, else, switch)

```csharp
int yas = 20;
if (yas >= 18)
{
    Console.WriteLine("Reşitsiniz.");
}
else
{
    Console.WriteLine("Reşit değilsiniz.");
}
```

### c. Döngüler (for, while, foreach)

```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine("Merhaba");
}
```

### d. Sınıflar ve Nesneler

```csharp
class Araba
{
    public string marka;
    public int modelYili;

    public void HareketEt()
    {
        Console.WriteLine("Araba hareket ediyor.");
    }
}

Araba araba1 = new Araba();
araba1.marka = "Toyota";
araba1.modelYili = 2020;
araba1.HareketEt();
```

### e. Kalıtım (Inheritance)

```csharp
class Hayvan
{
    public void SesCikar()
    {
        Console.WriteLine("Hayvan sesi çıkardı.");
    }
}

class Kopek : Hayvan
{
    public void Havla()
    {
        Console.WriteLine("Köpek havladı.");
    }
}
```

### f. Arayüzler (Interfaces)

```csharp
interface IUcan
{
    void Uc();
}

class Kus : IUcan
{
    public void Uc()
    {
        Console.WriteLine("Kuş uçuyor.");
    }
}
```

### g. Delegeler (Delegates)

```csharp
public delegate void MesajHandler(string mesaj);

class Program
{
    static void Main(string[] args)
    {
        MesajHandler handler = MesajYaz;
        handler("Merhaba C#");
    }

    static void MesajYaz(string mesaj)
    {
        Console.WriteLine(mesaj);
    }
}
```

### h. Linq (Language Integrated Query)

```csharp
int[] sayilar = { 1, 2, 3, 4, 5 };
var ciftSayilar = from s in sayilar
                  where s % 2 == 0
                  select s;

foreach (var sayi in ciftSayilar)
{
    Console.WriteLine(sayi);
}
```

## 3. C# ve .NET Platformu
C#, .NET platformunun bir parçasıdır ve .NET Framework, .NET Core veya .NET 5+ ile çalışır. C# dili, masaüstü, web ve bulut tabanlı uygulamalardan oyun geliştirmeye kadar geniş bir kullanım alanına sahiptir.

## 4. C#’ın Kullanım Alanları
C# dilinin kullanıldığı başlıca alanlar şunlardır:
- **Masaüstü Uygulamaları:** Windows Forms, WPF.
- **Web Geliştirme:** ASP.NET Core.
- **Oyun Geliştirme:** Unity oyun motoru.
- **Bulut Uygulamaları:** Azure tabanlı çözümler.
- **Mobil Uygulamalar:** Xamarin/MAUI.

## 5. C# ile İlgili İleri Konular
- **Asenkron Programlama:** `async` ve `await` ile zaman uyumsuz işlemler.
- **Task Paralelleştirme:** Paralel programlama.
- **Generics (Jenerikler):** Tip bağımsız sınıflar ve metodlar.
- **Exception Handling:** Hata yönetimi (`try`, `catch`, `finally`).

---

C# dili, geniş kullanım alanı ve güçlü özellikleri ile modern yazılım geliştirmede kritik bir role sahiptir.
