# ProStock - Türkcell Bayi Envanter Yönetim Sistemi

ProStock, Türkcell bayileri için geliştirilmiş kapsamlı bir envanter ve satış yönetim sistemidir.

## Özellikler

### 📦 Ürün Yönetimi
- Ürün ekleme, düzenleme, silme
- Barkod ile ürün arama
- Kategori bazlı ürün organizasyonu
- Stok takibi ve uyarı sistemi
- Düşük stok bildirimleri

### 💰 Satış Yönetimi
- Hızlı satış işlemleri
- Barkod okuyucu desteği
- Satış geçmişi ve raporlama
- Günlük/haftalık/aylık ciro takibi

### 💸 Gider Yönetimi
- Gider kategorileri oluşturma ve yönetimi
- Gider ekleme, düzenleme, silme
- Vade tarihi takibi
- Yaklaşan ödemeler uyarı sistemi
- Aylık/yıllık gider istatistikleri
- Bekleyen ve geciken ödeme takibi

### 📊 Dashboard ve Raporlama
- Gerçek zamanlı istatistikler
- Satış ve gider analizi
- Stok durumu özeti
- Yaklaşan ödemeler bildirimi
- Hızlı erişim menüleri

### 🔧 Teknik Özellikler
- Responsive tasarım (mobil uyumlu)
- Türkçe arayüz
- PostgreSQL veritabanı desteği
- Modern React.js frontend
- Node.js/Express backend
- Güvenli kullanıcı girişi

## Kurulum

### Gereksinimler
- Node.js (v20+)
- PostgreSQL
- npm veya yarn

### Adımlar

1. **Repository'yi klonlayın:**
```bash
git clone https://github.com/ckurudal/prostock-inventory.git
cd prostock-inventory
```

2. **Bağımlılıkları yükleyin:**
```bash
npm install
```

3. **Veritabanını ayarlayın:**
```bash
# PostgreSQL veritabanı oluşturun
createdb prostock

# Veritabanı şemasını oluşturun
npm run db:push
```

4. **Çevre değişkenlerini ayarlayın:**
```bash
# .env dosyası oluşturun
DATABASE_URL=postgresql://username:password@localhost:5432/prostock
```

5. **Uygulamayı başlatın:**
```bash
npm run dev
```

Uygulama http://localhost:5000 adresinde çalışacaktır.

## Varsayılan Giriş Bilgileri

- **Kullanıcı Adı:** admin
- **Şifre:** 123456

## Teknoloji Stack

### Frontend
- React.js
- TypeScript
- Tailwind CSS
- Shadcn/ui komponentleri
- TanStack Query
- Wouter (routing)

### Backend
- Node.js
- Express.js
- TypeScript
- Drizzle ORM
- PostgreSQL

## API Endpoints

### Ürünler
- `GET /api/products` - Tüm ürünleri listele
- `POST /api/products` - Yeni ürün ekle
- `PUT /api/products/:id` - Ürün güncelle
- `DELETE /api/products/:id` - Ürün sil

### Giderler
- `GET /api/expenses` - Tüm giderleri listele
- `POST /api/expenses` - Yeni gider ekle
- `PUT /api/expenses/:id` - Gider güncelle
- `DELETE /api/expenses/:id` - Gider sil
- `GET /api/expenses/stats` - Gider istatistikleri
- `GET /api/expenses/upcoming` - Yaklaşan ödemeler

### Gider Kategorileri
- `GET /api/expense-categories` - Tüm kategorileri listele
- `POST /api/expense-categories` - Yeni kategori ekle
- `PUT /api/expense-categories/:id` - Kategori güncelle
- `DELETE /api/expense-categories/:id` - Kategori sil

## Kullanım

### Gider Yönetimi
1. Dashboard'dan "Gider Yönetimi" butonuna tıklayın
2. "Gider Ekle" ile yeni gider oluşturun
3. Kategori, tutar, vade tarihi ve notlar ekleyin
4. "Kategori Yonet" ile gider kategorilerini düzenleyin

### Ürün Yönetimi
1. Sidebar'dan "Ürünler" menüsüne gidin
2. "Ür�n Ekle" ile yeni ür�n ekleyin
3. Barkod, kategori, fiyat bilgilerini girin
4. Stok miktarı ve minimum stok seviyesi belirleyin

### SatDıŖ|��������ɤ(ĸ��M��1��]��Ȉ������������ͅ��|���sana ˧idin
2. Barkod okuyucu ili ürün ekleyin
3. Satış işlemini tamamlayın

## KatC�kıda Bulunma

1. Bu repository'yi fork edin
2. Feature branch oluŝturun (`git checkout -b feature/yeni-ozellik`)
3. Değişikli�Lerinizi commit edin (!git commit -am 'Yeni öellik eklendi'`)
4. Branch'ninizipush edin (`git push origin feature/yeni-ozellik)
5. Pull Request oluşturun

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## Destek

Herhangi bir sorun yaşarsanız, GitHub Issues bölümünden bildirin.

---

**ProStock** - Türkcell bayileri için güçlü envanter yönetimi