# Fegn 3.3.1

Fegn, Wholf dilinde entegrasyon ve veri yönetimi için kullanılan modern ve güçlü bir kütüphanedir.

## Yeni Özellikler

- Modern API entegrasyonu
- Gelişmiş veri yönetimi
- Gelişmiş olay yönetimi
- WebSocket desteği
- Cache yönetimi
- Veri doğrulama
- Gelişmiş hata yönetimi
- Stream desteği
- Event sourcing
- Asenkron programlama

## Kurulum

```wholf
fort import "Fegn-3.3.1"
```

## Kullanım Örnekleri

### Modern API Entegrasyonu

```wholf
// Modern API entegrasyonu
fegn Api {
    // GET isteği
    get: ("/users") => {
        Console.log("Kullanıcılar alındı")
    },
    
    // POST isteği
    post: ("/users", {
        name: "Ahmet",
        email: "ahmet@example.com"
    }) => {
        Console.log("Kullanıcı eklendi")
    },
    
    // Stream desteği
    stream: ("/events") => {
        Console.log("Yeni olay alındı")
    }
}
```

### Gelişmiş Veri Yönetimi

```wholf
// Veri yönetimi
fegn Data {
    // Veri ekle
    add: ("users", {
        name: "Ahmet",
        email: "ahmet@example.com"
    }) => {
        Console.log("Kullanıcı eklendi")
    },
    
    // Veri al
    get: ("users", {
        email: "ahmet@example.com"
    }) => {
        Console.log("Kullanıcı bulundu")
    },
    
    // Stream desteği
    pipe: (data) => {
        Console.log("Veri akışı")
    }
}
```

## Lisans

MIT License
