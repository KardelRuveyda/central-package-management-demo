echo "# Central Package Management Demo (.NET)

Bu repo, **.NET projelerinde Central Package Management (CPM)** kullanımını göstermek için hazırlanmıştır.  
Küçük bir class library (Demo.Core) ve test projesi (Demo.Tests) içerir.  
Ayrıca Directory.Packages.props dosyası üzerinden paket versiyonlarının nasıl merkezi yönetildiğini örnekler.

## 🚀 İçerik
- Demo.Core → Örnek class library
- Demo.Tests → xUnit tabanlı test projesi
- Directory.Packages.props → Merkezi paket yönetimi ayarları
- Directory.Build.props → Ortak build ayarları

## ⚙️ CPM Nedir?
Central Package Management (CPM), NuGet paket versiyonlarının her .csproj dosyasında ayrı ayrı tanımlanması yerine, tek bir merkezi dosyada (Directory.Packages.props) tutulmasını sağlar.

Avantajları:
- Tek noktadan yönetim
- Tutarlılık
- Kolay güncelleme
- Daha az merge conflict

## Kullanım
git clone https://github.com/<kullanıcı-adın>/central-package-management-demo.git
cd central-package-management-demo
dotnet restore
dotnet build
dotnet test

## Klasör Yapısı
Demo.Core/
Demo.Tests/
DemoCPM.sln
Directory.Build.props
Directory.Packages.props

## 📘 Kaynaklar
- NuGet CPM Docs
- .NET CLI Docs

## 📌 Lisans
MIT" > README.md
