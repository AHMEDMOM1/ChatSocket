# 💬 **C# ile Socket Kullanarak Sohbet Uygulaması (Chat-App)**

C# diliyle **socket programlama** kullanılarak geliştirilmiş basit bir **sohbet uygulamasıdır**.
Kullanıcılar, bir **sunucuya bağlanarak** metin mesajları aracılığıyla birbirleriyle **gerçek zamanlı iletişim** kurabilirler.

---

## ⚙️ **Gereksinimler**

Uygulamayı çalıştırmak için aşağıdaki araçlara ihtiyacınız vardır:

* 🧩 Visual Studio 2019 veya üzeri
* 💻 .NET Framework 6

---

## 🚀 **Kurulum ve Kullanım Adımları**

1. 📥 Projeyi (repository) yerel makinenize klonlayın.
2. 🧭 **Chat-app.sln** dosyasını Visual Studio’da açın.
3. 🏗️ Çözümü derleyin (Build Solution).
4. 🔌 **Server** projesini başlatarak sunucuyu çalıştırın.
5. 💬 **Client** projesini başlatarak bir veya birden fazla istemci açın.
6. 🌐 İstemci arayüzünde sunucunun **IP adresini** ve **port numarasını** girin.
7. ✅ Bağlantı kurulduktan sonra mesaj göndermeye başlayabilirsiniz!

---

## ✨ **Özellikler**

* 👥 Birden fazla istemci aynı anda sunucuya bağlanabilir.
* ⚡ Gerçek zamanlı mesaj gönderimi ve alımı.
* 🧵 Her istemci için ayrı bir iş parçacığı (thread) oluşturulur.
* 🔐 Her istemciye benzersiz bir kimlik (ID) atanır.

---

## 🧠 **Mimari Yapı**

Uygulama, klasik bir **istemci-sunucu (client-server)** mimarisi üzerine inşa edilmiştir.

* **Sunucu (Server)** belirli bir port üzerinden gelen bağlantıları dinler.
* **İstemci (Client)** sunucuya bağlandığında, sunucu istemciyi yönetmek için yeni bir **thread** başlatır.
* İstemciler arasındaki tüm iletişim **TCP soketleri (TCP sockets)** üzerinden gerçekleşir.
* Mesajlar **byte dizileri** olarak iletilir ve **UTF-8** kodlamasıyla çözümlenir.

---

## 🧩 **Teknolojiler**

| Bileşen      | Açıklama                    |
| ------------ | --------------------------- |
| 🖥️ C#       | Uygulama dili               |
| 🔌 Socket    | İstemci-sunucu iletişimi    |
| ⚙️ .NET 6    | Framework                   |
| 🧠 Threading | Eşzamanlı bağlantı yönetimi |
