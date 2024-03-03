# Deploy Producer dengan Docker Compose

## Overview

Layanan producer adalah layanan yang berfungsi untuk melakukan pengambilan data pada jaringan GEOFON, memparsing ke struktur data JSON, dan mengirimnya ke Kafka.

## Requirements

- VM dengan Docker dan Docker Compose terinstal.
- Firewall pada VM harus mengizinkan traffic ingress pada port `8000`.

## Deployment Steps

1. **Konfigurasi Producer**

   - Pastikan environment variables pada `docker-compose.yaml` sudah benar.

2. **Menjalankan Producer**

   - Navigasikan ke direktori tempat file `docker-compose.yaml` berada.
   - Jalankan perintah berikut untuk mendeploy Producer:

     ```sh
     docker-compose up -d
     ```

   - Periksa status container untuk memastikan Producer berjalan dengan baik:

     ```sh
     docker-compose ps
     ```
