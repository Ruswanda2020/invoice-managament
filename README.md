#Aplikasi Invoice Management#

Aplikasi ini di pakai Untuk mengelola Invoice dan Menyambungkan dengan berbagai metode 
diantara metode Pembayaran yang akan di support antara lain :

*Virtual Account Bank
    *Bank BNI
    *Bank CIMB
    *Bank BCA
*e-wallet 
    *Ovo
    *GoPay
*QR Payment
    *QRIS

#cara setup database#
docker run --rm \
--name invoice-db \
-e POSTGRES_USER=invoicedb \
-e POSTGRES_PASSWORD=wAKTfT7DlWmuzRpPbC9hNH7NLBKGph \
-e PGDATA=/var/lib/postgresql/data/pgdata \
-v ./invoicedb-data:/var/lib/postgresql/data \
-p 5432:5432 \
postgres:13



