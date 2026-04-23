# Project: ecommerce-website

A simple e-commerce website for a small business which sells apparels. Users can search for products, browse available products, view product details, upload product images, and access backend services with PostgreSQL, Redis, Docker, and JWT-based admin authentication.

## Tools used for the project

- Frontend: HTML, CSS, JavaScript
- Backend: Python Flask
- Database: PostgreSQL
- Cache: Redis
- Containerization: Docker, Docker Compose
- Authentication: JWT

## Features

- Home page with featured products
- Products listing page
- Product details
- Image upload
- PostgreSQL-backed product storage
- Redis caching for home and products APIs
- JWT-protected product upload
- Docker Compose multi-container setup

## API overview

The backend exposes API routes for:

1. `/` – health check
2. `/home/` – featured products
3. `/products?page=1` – products listing
4. `/uploads/<filename>` – serve uploaded images
5. `/upload` – upload image
6. `/login` – admin login
7. `/add-product` – protected product creation

## Run locally with Docker Compose

From the project root:

```bash
docker compose down -v
docker compose up -d --build