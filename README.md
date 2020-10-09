# Promos-for-our-e-commerce
Divisi e-commerce kita ingin memprediksi apakah user- user yang sedang mengunjungi halaman website yang baru akan mengklik banner promo (ads) di halaman tersebut atau tidak berdasarkan feature yang ada. saya dimina tolong buatkan machine learning model untuk menyelesaikan permasalahan dari e-commerce ini

Step 1:
Aku akan membuat machine learning model untuk menyelesaikan permasalahan dari e-commerce divisi kantor.
Adapun feature - feature dalam dataset ini adalah :
'Daily Time Spent on Site' : lama waktu user mengunjungi site (menit)
'Age' : usia user (tahun)
'Area Income' : rata - rata pendapatan di daerah sekitar user
'Daily Internet Usage' : rata - rata waktu yang dihabiskan user di internet dalam sehari (menit)
'Ad Topic Line' : topik/konten dari promo banner
'City' : kota dimana user mengakses website
'Male' : apakah user adalah Pria atau bukan
'Country' : negara dimana user mengakses website
'Timestamp' : waktu saat user mengklik promo banner atau keluar dari halaman website tanpa mengklik banner
'Clicked on Ad' : mengindikasikan user mengklik promo banner atau tidak (0 = tidak; 1 = klik).
Di proyek ini, aku diharapkan untuk membuat machine learning model sesuai dengan prosedur machine learning yang sudah disharing sebelumnya. Jadi, tahap - tahap yang perlu dilakukan adalah (langkah ke-1) terlebih dahulu

Data eksplorasi dengan head(), info(), describe(), shape

Step 2:
Data eksplorasi dengan dengan mengecek korelasi dari setiap feature menggunakan fungsi corr()
Data eksplorasi dengan mengecek distribusi label menggunakan fungsi groupby() dan size()

Step 3: 
Data eksplorasi dengan visualisasi:
Jumlah user dibagi ke dalam rentang usia menggunakan histogram (hist()), gunakan bins = data.Age.nunique() sebagai argumen. nunique() adalah fungsi untuk menghitung jumlah data untuk setiap usia (Age).
Gunakan pairplot() dari seaborn modul untuk menggambarkan hubungan setiap feature. 

Step 4:
Cek missing value

step 5:
Lakukan pemodelan dengan Logistic Regression, gunakan perbandingan 80:20 untuk training vs testing :
Deklarasikan data ke dalam X dengan mendrop feature/variabel yang bukan numerik, (type = object) dari data (Logistic Regression hanya dapat memproses numerik variabel). Assign Target/Label feature dan assign sebagai y
Split X dan y ke dalam training dan testing dataset, gunakan perbandingan 80:20 dan random_state = 42
Assign classifier sebagai logreg, kemudian fit classifier ke X_train dan predict dengan X_test. Print evaluation score.

step 6:
Print Confusion matrix dan classification report
