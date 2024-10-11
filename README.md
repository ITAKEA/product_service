# Product Catalog Service

Dette repository indeholder en Flask-baseret Product Catalog Service, der henter produkter fra et eksternt API og giver funktionalitet til at søge, filtrere og kategorisere produkter.

## Kom godt i gang

Følg disse trin for at få en kopi af projektet op at køre på din lokale maskine til udviklings- og testformål.

### Installation

1. Klon dette repository til din lokale maskine:

   ```bash
   git clone https://github.com/din-bruger/product-catalog-service.git
   cd product-catalog-service
   ```

2. Installer de nødvendige Python-pakker:

   ```bash
   pip install flask requests
   ```

3. Kør applikationen:

   ```bash
   python app.py
   ```

## Anvendelse

Når applikationen kører, kan du få adgang til følgende endpoints for at interagere med produktkataloget:

### Endpoints

- **GET /products**

  Returnerer en liste over alle produkter.

  ```bash
  curl http://localhost:5000/products
  ```

- **GET /products/search?name=<søgenavn>**

  Søger efter produkter ved navn. <søgenavn> er en parameter, der filtrerer produkter baseret på deres navn.

  ```bash
  curl "http://localhost:5000/products/search?name=telefon"
  ```

- **GET /products/category/<kategorienavn>**

  Returnerer produkter, der tilhører en bestemt kategori. <kategorienavn> er det navn, der kategoriserer produkter.

  ```bash
  curl http://localhost:5000/products/category/electronics
  ```

## Licens

Dette projekt er licenseret under MIT-licensen - se [LICENSE.md](LICENSE.md) for detaljer.

## Forfatter

- **Claus Bové** - [Din GitHub-profil](https://github.com/din-bruger)
