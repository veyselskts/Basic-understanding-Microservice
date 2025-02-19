# E-Commerce Market Service

## 📋 Proje Hakkında
Bu proje, modern bir e-ticaret platformunun market servis bileşenidir. Ürün yönetimi, stok kontrolü ve fiyatlandırma gibi temel e-ticaret fonksiyonlarını sağlar.

## 🚀 Özellikler
- Ürün yönetimi (ekleme, güncelleme, silme, listeleme)
- Stok takibi
- Fiyat yönetimi
- Kategori bazlı ürün organizasyonu

## 🛠 Teknolojiler
- Java 17
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Docker
- Maven

## 📦 Kurulum

### Ön Gereksinimler
- Java 11 veya üzeri
- Docker ve Docker Compose
- Maven

### Projeyi Çalıştırma

1. Projeyi klonlayın:
   ```bash
   git clone https://github.com/yourusername/ecommerce-market-service.git
   cd ecommerce-market-service
   ```


2. Maven ile projeyi derleyin:
   ```bash
   mvn clean install
   ```

3. Docker container'ları başlatın:
bash
docker-compose up -d


4. Uygulama varsayılan olarak `http://localhost:8080` adresinde çalışacaktır.

## 🔧 Konfigürasyon

### Environment Variables

```bash
MYSQL_ROOT_PASSWORD=root
MYSQL_DATABASE=ecommerce
MYSQL_USER=ecommerce
MYSQL_PASSWORD=ecommerce

## 📚 API Dokümantasyonu
API dokümantasyonuna `http://localhost:8080/swagger-ui.html` adresinden erişebilirsiniz.

### Temel Endpoints
- `GET /api/v1/products`: Tüm ürünleri listeler
- `GET /api/v1/products/{id}`: Belirli bir ürünü getirir
- `POST /api/v1/products`: Yeni ürün ekler
- `PUT /api/v1/products/{id}`: Ürün günceller
- `DELETE /api/v1/products/{id}`: Ürün siler
