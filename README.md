# İnternet Programcılığı 2 — Final Projesi

Bu proje, İnternet Programcılığı II dersinin final ödevi kapsamında geliştirilmiştir.  
Ürün ve kategori yönetimi yapılabilen, ASP.NET Web API tabanlı bir backend ile Angular tabanlı bir frontend uygulamasından oluşmaktadır.

---

## 🗂️ Proje Yapısı

| Klasör | İçerik |
|--------|--------|
| `IPF2/` | ASP.NET Web API — Backend & API katmanı |
| `IP2Final/` | Angular 13 — Frontend uygulaması |

---

## 🛠️ Teknolojiler

**Backend**
- ASP.NET Web API (C#)
- Entity Framework (Database-First)
- SQL Server

**Frontend**
- Angular 13
- Angular Material
- TypeScript

---

## 📐 Veritabanı Şeması

![Veritabanı Şeması](https://i.ibb.co/gDDgzQV/resim-2023-06-16-213840052.png)

---

## 🔌 API Yapısı

![API Yapısı](https://i.ibb.co/xSMRnxN/image.png)

---

## 📋 API Endpoint'leri

### Ürün

| Method | Endpoint | Açıklama |
|--------|----------|----------|
| `GET` | `/api/urunliste` | Tüm ürünleri listeler |
| `GET` | `/api/urunbyid/{urunId}` | ID'ye göre ürün getirir |
| `POST` | `/api/urunekle` | Yeni ürün ekler |
| `PUT` | `/api/urunduzenle` | Ürün bilgilerini günceller |
| `DELETE` | `/api/urunsil/{urunId}` | Ürün siler |
| `POST` | `/api/urunresimguncelle` | Ürün resmini günceller |

### Kategori

| Method | Endpoint | Açıklama |
|--------|----------|----------|
| `GET` | `/api/kategoriliste` | Tüm kategorileri listeler |
| `GET` | `/api/kategoribyid/{katId}` | ID'ye göre kategori getirir |
| `POST` | `/api/kategoriekle` | Yeni kategori ekler |
| `PUT` | `/api/kategoriduzenle` | Kategori bilgilerini günceller |
| `DELETE` | `/api/kategorisil/{katId}` | Kategori siler |

### Kayıt (Ürün–Kategori İlişkisi)

| Method | Endpoint | Açıklama |
|--------|----------|----------|
| `GET` | `/api/kategoriurunliste/{katId}` | Kategoriye ait ürünleri listeler |
| `GET` | `/api/urunkategoriliste/{urunId}` | Ürünün bağlı olduğu kategorileri listeler |
| `POST` | `/api/kayitekle` | Ürünü kategoriye ekler |
| `DELETE` | `/api/kayitsil/{kayitId}` | Ürün–kategori kaydını siler |

---
