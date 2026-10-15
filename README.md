# Limonmatik

Limonmatik ürünü için Next.js (App Router) tabanlı tanıtım/vitrin sitesi. UI dili livelarq.com referans alınarak kurulmuştur; bu fazda gerçek ödeme/checkout yoktur (mock fiyat/sepet).

## Geliştirmeye başlama

```bash
npm install
npm run dev
```

Site varsayılan olarak http://localhost:3000 adresinde açılır.

## Diğer komutlar

```bash
npm run build      # production build
npm run start       # production build'i çalıştırır (önce build gerekir)
npm run lint         # ESLint
npm run typecheck   # TypeScript tip kontrolü
```

## Proje yapısı

- `app/` — sayfalar (`/`, `/urun`, `/hikayemiz`, `/sss`, `/iletisim`) ve paylaşılan bileşenler (`app/_components/`).
- `content/copy.ts` — tüm Türkçe UI metinleri tek noktadan yönetilir.
- `lib/product.ts` — mock ürün/varyant/fiyat verisi.
- `public/images/` — PDF'ten çıkarılan ürün görselleri ve üretilen bölüm arkaplanları.
- `docs/` — planlama ve analiz dokümanları (PDF analizi, livelarq UI analizi, karşılaştırma planı, PayTR entegrasyon araştırması, görsel envanteri).

## Bilinmesi gerekenler

- Fiyat ve sepet davranışı **demo/mock**'tur; gerçek bir sipariş oluşturmaz.
- PayTR entegrasyonu bu fazda kapsam dışıdır (bkz. `docs/04-paytr-entegrasyon-arastirmasi.md` başındaki not); ileride gerçek ödeme eklenirse referans olarak kullanılabilir.
- Üründeki bazı iddialar (BPA, hijyen, dayanıklılık vb.) üretici belgesiyle doğrulanana kadar sitede kesin ifade olarak kullanılmamıştır; bkz. `docs/01-pdf-analizi.md`.
# limonmatik-website
