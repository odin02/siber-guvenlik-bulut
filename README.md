# Bulut Bilişim ve Siber Güvenlik Projesi 🛡️

Manisa Celal Bayar Üniversitesi Büyük Veri Analistliği Programı - Bulut Bilişim ve Siber Güvenlik Dersi Projesi.

## 🚀 Proje Hakkında
Bu projede, AWS üzerindeki S3 depolama alanını elle oluşturmak yerine "Infrastructure as Code" (IaC) yaklaşımıyla yani kod yazarak (`main.tf` ile Terraform kullanarak) ayağa kaldırdım. Güvenliği en baştan ele almak için GitHub Actions CI/CD hattına **Checkov** güvenlik tarayıcısını entegre ettim. 

Sistemde bilerek açık bıraktığım "Herkese Açık (Public) S3" zafiyetini Checkov anında yakaladı ve pipeline'ı durdurdu. Ardından kodumu güncelleyip (privatelaştırarak ve şifrelemeyi açarak) güvenli versiyonu tekrar gönderdim ve sistem hatasız bir şekilde başarıyla tamamlandı.

## 🛠️ Kullanılan Teknolojiler
* Terraform (IaC)
* AWS S3
* Checkov (Statik Kod Analizi / SAST)
* GitHub Actions (CI/CD Otomasyonu)

## 📄 Rapor ve Dokümantasyon
* **Güvenlik Raporu:** [Siber_Guvenlik_Raporu.pdf](./Siber_Guvenlik_Raporu.pdf)

---
## 🤖 Yapay Zekâ ve Akademik Dürüstlük Beyanı
Bu projenin kodlama, zafiyet analizi ve dokümantasyon aşamalarında fikir alışverişi amacıyla Yapay Zekâ Asistanı'ndan (LLM) destek alınmıştır. Tüm mimari kararlar, zafiyet giderme adımları ve testler bizzat tarafımca gerçekleştirilmiştir.
