
# Proje Başlığı

Bu proje, C# kullanarak bir TODO listesi uygulaması geliştirmeyi amaçlamaktadır. Kullanıcılar bu uygulama ile görevlerini ekleyebilir, düzenleyebilir ve silebilirler.

## Özellikler

- Görev ekleme, düzenleme ve silme.
- Görevleri tamamlandı olarak işaretleme.
- Veritabanına görevleri kaydetme.
- Kullanıcı dostu arayüz.

## Gereksinimler

Bu projeyi çalıştırmak için aşağıdaki gereksinimlere sahip olmanız gerekir:

- .NET 6.0 SDK
- Visual Studio 2022 veya Visual Studio Code

## Kurulum

Projeyi yerel makinenize kurmak için aşağıdaki adımları takip edin:

1. Bu repoyu klonlayın: 
   ```bash
   git clone https://github.com/kullaniciadi/proje-adi.git
   ```

2. Proje dizinine gidin:
   ```bash
   cd proje-adi
   ```

3. Bağımlılıkları yükleyin:
   ```bash
   dotnet restore
   ```

4. Uygulamayı çalıştırın:
   ```bash
   dotnet run
   ```

## Kullanım

Uygulamayı çalıştırdıktan sonra tarayıcınızdan aşağıdaki URL'yi ziyaret edin:

```
http://localhost:5000
```

## Katkıda Bulunma

Katkıda bulunmak için lütfen aşağıdaki adımları izleyin:

1. Repoyu fork edin.
2. Yeni bir branch oluşturun (`git checkout -b yeni-ozellik`).
3. Değişikliklerinizi commitleyin (`git commit -m 'Yeni özellik ekle'`).
4. Branch'e push edin (`git push origin yeni-ozellik`).
5. Bir Pull Request açın.

## Testler

Testleri çalıştırmak için şu komutu kullanabilirsiniz:

```bash
dotnet test
```

## Lisans

Bu proje [MIT Lisansı](https://opensource.org/licenses/MIT) ile lisanslanmıştır.
