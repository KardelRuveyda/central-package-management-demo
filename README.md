# Central Package Management Demo (.NET)

Bu repo, **.NET projelerinde Central Package Management (CPM)** kullanımını göstermek için hazırlanmıştır.  
Küçük bir class library (`Demo.Core`) ve test projesi (`Demo.Tests`) içerir.  
Ayrıca `Directory.Packages.props` dosyası üzerinden paket versiyonlarının nasıl merkezi yönetildiğini örnekler.

---

## 🚀 İçerik

- `Demo.Core` → Örnek class library projesi  
- `Demo.Tests` → xUnit tabanlı test projesi  
- `Directory.Packages.props` → Merkezi paket yönetimi ayarları  
- `Directory.Build.props` → Ortak build ayarları  

---

## ⚙️ CPM Nedir?

Central Package Management (CPM), NuGet paket versiyonlarının her `.csproj` dosyasında ayrı ayrı tanımlanması yerine, tek bir merkezi dosyada (`Directory.Packages.props`) tutulmasını sağlar.  

### Avantajları:
- Paket sürümlerini **tek bir dosyadan yönetme**  
- **Tutarlılık:** Tüm projelerde aynı sürüm  
- **Kolay güncelleme:** Bir satırı değiştirmek tüm projelere yansır  
- **Daha az merge conflict**  

---

## 🔧 Kullanım

Projeyi klonladıktan sonra:

```bash
git clone https://github.com/<kullanıcı-adın>/central-package-management-demo.git
cd central-package-management-demo
dotnet restore
dotnet build
dotnet test
``

## 📂 Klasör Yapısı

central-package-management-demo/
│
├── Demo.Core/               # Class library
├── Demo.Tests/              # Test projesi
├── DemoCPM.sln              # Solution dosyası
├── Directory.Build.props    # Ortak build ayarları
└── Directory.Packages.props # CPM için merkezi paket yönetimi


