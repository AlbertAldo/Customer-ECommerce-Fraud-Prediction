# Customer-ECommerce-Fraud-Prediction

Dataset taken from : https://www.kaggle.com/aryanrastogi7767/ecommerce-fraud-data

# Define Problems
- Dikarenakan transaksi fraud yang dilakukan customer, menyebabkan transaksi yang dilakukan fiktif, sehingga memicu adanya penggunaan cashback/promo sebagai kesempatan untuk mengambil keuntungan pada pihak tertentu.

# Goals
- Dapat menentukan customer seperti apa saja yang melakukan fraud.
- Cara untuk menghandle customer yang melakukan fraud.
- Mengurangi kerugian yang timbul akibat fraud tersebut.

# Feature Selection
- No_Transactions : Jumlah Transaksi
- No_Orders : Jumlah Orderan Barang
- No_Payments : Jumlah payments yang dilakukan
- Fraud : Customers termasuk dalam golongan Fraud atau Non-Fraud **(Target)**
- Total_transaction : Total transaksi yang terjadi pada customer tersebut
- Fail_transaction : Total transaksi yang gagal pada customer tersebut
- PaymentRegFail : Total payment yang gagal diregistrasi
- PaypalPayments : Pembayaran menggunakan Paypal
- ApplePayments : Pembayaran menggunakan Apple
- CardPayments : Pembayaran menggunakan Card
- BitcoinPayments : Pembayaran menggunakan Bitcoin
- JCB_16 : Metode Provider yang digunakan untuk pembayaran menggunakan JCB_16
- AmericanExp : Metode Provider yang digunakan untuk pembayaran menggunakan AmericanExp
- VISA_16 : Metode Provider yang digunakan untuk pembayaran menggunakan VISA_16
- Discover : Metode Provider yang digunakan untuk pembayaran menggunakan Discover
- Voyager : Metode Provider yang digunakan untuk pembayaran menggunakan Voyager
- VISA_13 : Metode Provider yang digunakan untuk pembayaran menggunakan VISA_13
- Maestro : Metode Provider yang digunakan untuk pembayaran menggunakan Maestro
- Mastercard : Metode Provider yang digunakan untuk pembayaran menggunakan Mastercard
- DC_CB : Metode Provider yang digunakan untuk pembayaran menggunakan DC_CB
- JCB_15 : Metode Provider yang digunakan untuk pembayaran menggunakan JCB_15
- OrdersFulfilled : Order yang sudah terpenuhi / selesai
- OrdersPending : Order yang masih dalam status pending
- OrdersFailed : Order yang sudah gagal
- Trns_fail_order_fulfilled : Order yang gagal tetapi statusnya sudah terpenuhi / selesai
- Duplicate_IP : IP yang terduplikat pada Customers
- Duplicate_Address : Address yang terduplikat pada Customers

# Conclusion
- Berdasarkan data yang diperoleh, untuk perbandingan Customers yang Fraud dan Non-Fraud yaitu sebesar 0.608392 untuk yang Non-Fraud dan 0.391608 Fraud, sehingga berfokus pada Accuracy dari Model Machine Learning.
- Untuk kasus Customer Fraud berdasarkan data ini, didapatkan Model terbaik dengan menggunakan Algoritma : SVM dengan menggunakan Parameter sebagai berikut : max_iter=400, probability=True, kernel='linear', C = 1.4, gamma = 10, class_weight = {0 : 0.4, 1 : 0.6}. Dengan hasil Accuracy Data Train 0.824561, dan hasil Accuracy Data Testing 0.827586.

# Recommendation
- Untuk mengurangi fraud yang ditimbulkan oleh Customer, maka perusahaan dapat menggunakan Machine Learning ini pada saat memverifikasi ID Customer, sehingga dapat memprediksi bahwa customer tersebut melakukan fraud atau tidak.
