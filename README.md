# Clustering-Kendaraan

## Formulasi Masalah
Pada kasus kali ini kita akan memprediksi apakah pelanggan tertarik untuk membeli kendaraan baru atau tidak berdasarkan dataset yang diberikan dan membentuk beberapa cluster dari beberapa feature yang mempengaruhi seseorang akan membeli kendaraan atau tidak.

## Exploratory Data Analysist dan PreProcessing Data
* Data Train Exploration
* Handling Outlier
* Replace Data Categorical
* Handling Missing Value
* Drop Feature
* Check Correlation
* Feature Selection
* Scalling

## Model 
Model yang digunakan pada kasus clustering kali ini adalah metode KMeans Clustering atau centroid based. Konsep dasar dari metode ini adalah melakukan inisialisasi jumlah K sebagai centroid terlebih dahulu, kemudian dilakukan perhitungan dan membandingkan jarak dari data ke centroid terdekat, kemudian centroid akan terupdate, iterasi ini akan terus dilakukan sampai centroid tidak melakukan update/perubahan lagi. Pada model ini saya insialisasi dengan class bernama K_Means yang memiliki parameter n_cluster (jumlah cluster), max_iter (iterasi maksimal), dan random_state(untuk inisialisasi centroid).

## Evaluasi Model
Metode yang digunakan dalam Evaluasi Model adalah elbow Method. Elbow Method digunakan untuk menentukan jumlah K yang optimal untuk model clustering, caranya dengan melihat penurunan nilai WCSS (Within Cluster Sum of Squares), yaitu nilai SSE antar setiap cluster dan centroid nya. nilai elbow yang optimal dapat dilihat dengan penurunan nilai WCSS yang stabil dan tidak menunjukkan penurunan yang turun drastis.
