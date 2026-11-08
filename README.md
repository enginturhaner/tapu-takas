# Tapu Takas

Monopoly Deal kurallarıyla, arkadaşlarla tarayıcıda oynanan online kart oyunu.

- Oyunu kuran kişi "Yeni oyun kur"a basar ve çıkan bağlantıyı arkadaşlarına gönderir.
- Arkadaşlar bağlantıyı açar, adlarını yazar ve "Katıl"a basar. Hesap gerekmez.
- Oyuncular birbirine doğrudan bağlanır (PeerJS / WebRTC). Doğrudan bağlantı kurulamazsa (ör. aynı Wi-Fi'de modem izin vermezse) mesajlar herkese açık bir MQTT sunucusu (EMQX / HiveMQ) üzerinden gider. Ayrı bir oyun sunucusu yoktur; oyunu kuranın tarayıcısı hakemdir ve oyun boyunca açık kalmalıdır.
- "Botlarla dene" ile internet bağlantısı olmadan tek başına da oynanabilir.

Tek dosyalık statik bir sayfadır (`index.html`); GitHub Pages ile yayınlanır.
