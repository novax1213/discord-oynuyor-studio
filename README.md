# Discord Oynuyor Studio

Discord profilindeki **Oynuyor** alanını Rich Presence ile düzenleyen Windows masaüstü uygulaması.

## İlk kurulum

1. [Discord Developer Portal](https://discord.com/developers/applications) sayfasını aç.
2. **New Application** ile bir uygulama oluştur. Discord'un üst başlıkta göstermesini istediğin adı ver.
3. **General Information** sayfasındaki **Application ID** değerini kopyala.
4. Görsel kullanacaksan **Rich Presence → Art Assets** bölümünde kare bir PNG/JPEG/WebP yükle. Verdiğin küçük harfli anahtarı uygulamadaki **Görsel** alanına yaz. Alternatif olarak herkese açık bir HTTPS görsel adresi kullan.
5. Discord'un masaüstü uygulamasını aç, `Discord-Oynuyor-Studio-1.0.0.exe` dosyasını çalıştır ve **Discord’da Göster** düğmesine bas.

> Discord masaüstü istemcisinde **Ayarlar → Etkinlik Gizliliği → Mevcut etkinliği durum mesajı olarak göster** açık olmalıdır.

## Geliştirme

```powershell
npm install
npm start
```

Test ve taşınabilir Windows paketi:

```powershell
npm test
npm run dist
```

## Gizlilik

Uygulama bot tokeni veya Discord parolası istemez. Ayarlar yalnızca bilgisayarda Electron kullanıcı verisi klasöründeki `ayarlar.json` dosyasında saklanır. Discord bağlantısı yerel IPC üzerinden açık Discord masaüstü istemcisine yapılır.
