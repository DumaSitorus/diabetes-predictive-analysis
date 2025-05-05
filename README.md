# Laporan Proyek Machine Learning - Duma Mora Arta Sitorus

## Domain Proyek

## Latar Belakang

Diabete Mellitus (DM) merupakan gangguan penyakit pada endokrin atau hormon yang merupakan hasil dari proses destruksi sel pankreas sehingga insulin mengalami kekurangan jumlah dalam tubuh. Diabetes mellitus merupakan salah satu masalah kesehatan yang berdampak pada produktivitas sehari-hari serta dapat menyebabkan kematian (Imelda, 2019). Diabetes sering disebabkan oleh faktor genetik, gaya hidup, lingkungan sosial, serta pelayanan kesehatan yang dalam jangka waktu tertentu mempengaruhi berbagai sistem organ tubuh yang disebut komplikasi (Lestari et al., 2019). Diabetes merupakan induk dari penyakit karena dapat menyebabkan komplikasi seperti hipertensi, penyakit jantung dan pembuluh darah, stroke, gagal ginjal dan kebutaan (Maulidah et al., 2021).

Machine learning merupakan aplikasi kecerdasan buatan dan ilmu komputer yang berfokus pada data dan algoritma untuk terus belajar seperti manusia serta meningkatkan akurasinya (Ginting, 2022). Machine learning efektif digunakan dalam dunia kesehatan dan salah satunya adalah deteksi dini penyakit. Sehingga machine learning dapat menjadi solusi untuk melakukan prediksi penyakit diabetes pada pasien berdasarkan data diagnosis . Melalui solusi ini, tenaga medis dapat terbantu dalam pengambilan keputusan yang lebih cepat dan tepat, pasien mendapatkan penanganan lebih dini sehingga risiko komplikasi dapat ditekan, serta instansi kesehatan dapat meningkatkan efisiensi layanan dengan memanfaatkan teknologi prediktif berbasis data.

Proyek machine leaning ini akan menerapkan metode klasifikasi untuk memprediksi apakah seseorang mengidap penyakit diabetes atau tidak. Dataset yang digunakan dalam proyek ini berasal dari Institut Nasional Penyakit Diabetes, Pencernaan dan Ginjal.Data berupa hasil pemeriksaan kesehatan pasien seperti jumlah kehamilan, kadar glukosa, tekanan darah, ketebalan kulit, kadar insulin, BMI, fungsi silsilah diabetes, serta usia(tahun). Data yang terdapat dalam dataset tersebut diambil dari pasien berjenis kelamin perempuan berusia minimal 21 tahun dan merupakan keturunan Indian Pima. Data akan dilatih menggunakan algoritma machine learning yaitu *Support Vector Machine*, *Boosting* (AdaBoost),  dan *Logistic Regression*.

## Daftar Pustaka

Ginting, R. G., Girsang, E., Ginting, J. B. ., & Hartono, H. (2022). ANALISIS DETERMINAN DAN PREDIKSI PENYAKIT DIABETES MELITUS TIPE 2 MENGGUNAKAN METODE MACHINE LEARNING: SCOPING REVIEW. Jurnal Maternitas Kebidanan, 7(1), 58-72. https://doi.org/10.34012/jumkep.v7i1.2538

Imelda, Sonta I. "Faktor-Faktor yang Mempengaruhi Terjadinya Diabetes Melitus di Puskesmas Harapan Raya Tahun 2018." Scientia Journal, vol. 8, no. 1, 2019, pp. 28-39, doi:10.5281/scj.v8i1.406.

Lestari, Zulkarnain, Sijid, & Aisyah, S. (2021). Diabetes Melitus: Review Etiologi, Patofisiologi, Gejala, Penyebab, Cara Pemeriksaan, Cara Pengobatan dan Cara Pencegahan. UIN Alauddin Makassar, 1(2), 237–241. Retrieved from http://journal.uin-alauddin.ac.id/index.php/psb

Maulidah, N., Supriyadi, R., Utami, D. Y., Hasan, F. N., Fauzi, A., & Christian, A. (2021). Prediksi Penyakit Diabetes Melitus Menggunakan Metode Support Vector Machine dan Naive Bayes. Indonesian Journal on Software Engineering (IJSE), 7(1), 63–68. https://doi.org/10.31294/ijse.v7i1.10279

## Business Understanding

Bagian laporan ini meliputi problem statement, goals, dan solution statement.

### Problem Statements

Masalah utama yang akan diselesaikan dalam proyek ini adalah bagaimana machine learning dapat membantu dunia medis dalam mendeteksi dini penyakit diabetes secara otomatis. Untuk mencapai tujuan tersebut, terdapat beberapa tantangan yang perlu diatasi, yaitu:
1. Bagaimana menetukan fitur-fitur yang paling berpengaruh terhadap hasil prediksi atau dignosis diabetes untuk meningkatkan akurasi model prediksi?
2. Bagaimana mempersiapkan data agar dapat digunakan untuk melatih dan mengevaluasi model dan memberikan kinerja yang optimal untuk melakukan prediksi diabetes?
3. Bagaimana menghasilkan model machine learning yang mampu memprediksi apakah seseorang mengidap diabetes melalui data pemeriksaan medis?
4. Bagaimana memastikan model yang telah dilatih cukup akurat dalam melakukan prediksi atau diagnosis diabetes?

### Goals

Tujuan utama dari proyek ini adalah menyelesaikan permasalahan yang telah diidentifikasi sebelumnya dalam problem statement, yaitu:
1. Memperoleh fitur atau variabel yang paling berpengaruh terhadap hasil prediksi untuk meningkatkan kinerja model.
2. Menghasilkan dataset yang bersih dari invalid value, missing value, outlier, memiliki proporsi seimbang dan terdistribusi normal untuk proses pelatihan dan memperolah model yang memiliki kinerja yang oprimal dalam memprediksi diabetes.
3. Menerapkan algoritma machine learning untuk tugas klasifikasi untuk menghasilkan model prediksi diabetes yang optimal.
4. Memperoleh hasil pengukuran evaluasi untuk memastikan model cukup optimal dalam melakukan prediksi atau diagnosis diabetes.

### Solution statements

Untuk menjawab permasalahan yang telah diidentifikasi sebelumnya dan mencapai tujuan dari proyek ini, diajukan beberapa solusi dengan pendekatan machine learning, yaitu:
1. Melakukan eksplorasi terhadap dataset untuk memahami data, hubungan antar fitur. Eksplorasi dilakukan dengan melihat informasi statistik dan melakukan visualisasi untuk memperoleh pengetahuan dari dataset.
2. Mendeteksi ketidaksesuaian data seperti invalid data, missing data, imbalance data serta outlier melalui solusi pertama. Melakukan teknik penanganan terhadap setiap ketidaksesuaian dalam data yang sesuai dengan kondisi data.
3. Menggunakan beberapa algoritma dalam pengembangan model klasifikasi prediksi diabetes seperti:
    1. Support Vector Machine (SVM)
    2. Boosting Algorithm (AdaBoostClassifier)
    3. Logistic Regression
4. Melakukan evaluasi serta perbandingan model yang dihasilkan dari setiap algoritma menggunakan metrik evaluasi yang relevan.

## Data Understanding
Dataset yang digunakan diperoleh dari repository penyedia dataset [Kaggle](https://www.kaggle.com/) yang bernama [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database).

Data berasal dari Institut Nasional Penyakit Diabetes, Pencernaan, dan Ginjal. Dataset ini dapat digunakan untuk memprediksi secara diagnostik apakah seorang pasien menderita diabetes atau tidak berdasarkan pengukuran diagnostik seperti jumlah kehamilan, kadar glukosa, tekanan darah, ketebalan kulit, kadar insulin, BMI, fungsi silsilah diabetes, serta usia(tahun).

 Data yang terdapat dalam dataset tersebut diambil dari pasien berjenis kelamin perempuan berusia minimal 21 tahun dan merupakan keturunan Indian Pima. Dataset terdiri dari 9 fitur (8 variabel + 1 target) dan 768 data pengukuran

### Variabel-variabel pada  Pima Indians Diabetes Database adalah sebagai berikut:
  *   **pregnancies**: Jumlah kehamilan
  *   **Glucose**: Kadar glukosa (gula) dalam plasma darah setelah 2 jam menjalani Oral Glucose Tolerance Test (OGTT).
  *   **BloodPressure**: Tekanan darah diastolik  dalam satuan mm Hg
  *   **SkinThickness**: Tebal lipatan kulit pada bagian Trisep (lengan atas belakang) dalam satuan milimeter(mm).
  *   **Insulin**: Kadar insulin dalam darah selama 2 jam setelah melakukan OGTT, diukur dalam satuan mikro unit/milimeter(mU/ml)
  *   **BMI**:Body Mass Index (menyatakan proporsional berat badan terhadap tinggi badan seseorang) dalam satuan kilogram/meter persegi(kg/m^2)
  *   **DiabetesPedigreeFunction**: Ukuran probabilitas turunan genetik terhadap diabetes
  *   **Age**: Usia dalam tahun
  *   **Outcome**: bernilai 0 (untuk yang bukan penderita diabetes) dan 1 (untuk penderita diabetes).

### Exploratory Data Analysis
#### 1. Informasi dan Statistik Dataset
<img width="323" alt="1_dataset-info" src="https://github.com/user-attachments/assets/982bdeea-0fde-4865-b1b9-37eed67458ad" />

Keterangan:
- Dataset terdiri dari 9 variabel dengan 1 variabel target yaitu outcome.
- Dataset terdiri atas 768 baris data yang bertipe integer dan float.
- Dataset tidak memiliki missing value sehingga tidak perlu melakukan penanganan missing value.

<img width="761" alt="2_dataset-statistics" src="https://github.com/user-attachments/assets/792246ee-bd13-40f7-80f7-4ffb3104fb59" />

Keterangan:

**1.   Pregnancies:**
  *   Jumlah kehamilan minimal pasien adalah 0. Hal ini mungkin karena pasien belum menikah atau belum pernah melahirkan sebelumnya.
  *   Jumlah kehamilan terbanyak adalah 17. Data ini diragukan dan mengindikasikan kemungkinan outlier sehingga perlu pemeriksaan dengan analisis lanjutan terhadap outlier pada data.
  *   Rata-rata jumlah kehamilan adalah 4 kali (hasil pembulatan)

**2.   Glucose:**
  *   Jumlah kadar gula darah minimal pasien dalam dataset adalah 0. Hal ini tidak mungkin secara biologis, kemungkinan terjadi data error karena missing value sehingga perlu penanganan lebih lanjut.
  *   Jumlah kadar gula darah terbanyak adalah 199. meskipun angka ini sangat tinggi tapi ini mungkin saja terjadi.
  *   Rata-rata jumlah kehamilan adalah 120.89 mg/dL.

**3.   BloodPressure:**
  *   Jumlah Tekanan darah terendah pasien adalah 0 mmHg. Hal ini tidak mungkin secara biologis, kemungkinan terjadi data error karena missing value sehingga perlu penanganan lebih lanjut.
  *   Jumlah tekanan darah tertinggi adalah 122 mmHg. Data ini diragukan dan mengindikasikan kemungkinan outlier sehingga perlu pemeriksaan dengan analisis lanjutan terhadap outlier pada data.
  *   Rata-rata tekanan darah adalah 69.105469 mmHg.

**4.   SkinThickness:**
  *   Jumlah Skin Thickness terkecil pasien adalah 0. Hal ini tidak mungkin karena manusia pasti memiliki lemak, kemungkinan terjadi data error karena missing value sehingga perlu penanganan lebih lanjut.
  *   Jumlah Skin Thickness terbesar adalah 99 mm (hampir 10cm). Hal ini mungkin saja akan tetapi sangat jarang kecuali pasien merupakan pasien obesitas parah. Sehingga data ini diragukan dan mengindikasikan outlier dan perlu pemeriksaan dengan analisis lebih lanjut.
  *   Rata-rata Skin Thickness adalah 20.5 mm.

**5.   Insulin:**
  *   kadar insulin minimal pasien adalah 0 mU/ml. Hal ini mungkin terjadi jika pankreas sama sekali tidak memproduksi insulin yang dapat terjadi pada penderita diabetes tipe 1 berat. akan tetapi perlu dilakukan pemeriksaan lebih lanjut untuk memastikan tidak adanya data error karena missing value.
  *   kadar insulin terbanyak adalah 846 mU/ml. Hal ini mungkin terjadi pada kondisi dimana pasien memiliki masalah pada pankreas yang menyebabkan peningkatan produksi insulin seperti pada penderita tumor pankreas, obesitas, sindrom metabolik berat. Namun memungkinkan juga terjadi kekeliruan dalam data. sehingga perlu pemeriksaan dengan analisis lanjutan terhadap outlier pada data.
  *   Rata-rata kadar insulin adalah 79.79 mU/ml.

**6.   BMI:**
  *   BMI minimal pasien adalah 0 kg/m^2. 0. Hal ini sangat tidak mungkin, kemungkinan terjadi data error karena missing value sehingga perlu penanganan lebih lanjut.
  *   BMI tertinggi adalah 67.1 kg/m^2. Data cukup tinggi tetapi mungkin terjadi pada penderita diabetes ekstrim, diperlukan analisis lanjutan terhadap outlier pada data BMI.
  *   Rata-rata BMI adalah 31.99 kg/m^2.

**7.   DiabetesPedigreeFunction:**
  *   Probabilitas turunan genetik penderita diabetes terkecil adalah 0. Hal ini mungkin terjadi.
  *   Probabilitas tujutann genetik penderita diabetes tertinggi adalah 2.42. Hal ini mungkin saja terjadi namun masih sangat tinggi sehingga perlu pemeriksaan kemungkinan outlier lebih lanjut.
  *   Rata-rata Probabilitas turunan genetik penderita diabetes dalam dataset adalah 0.47.

**8.   Age:**
  *   Usia pasien yang dilakukan pengukuran diagnostik berkisar dari 21-81 tahun.
  *   Rata-rata usia pasien adalah 33 tahun (hasil pembulatan)

**9.   Outcome:**
  *   Bernilai 1 jika pasien menderita diabetes
  *   Bernilai 0 jika pasien tidak menderita diabetes

Kesimpulan:
- Terdapat indikasi error data pada fitur Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction. Hal ini perlu ditelusuri lebih lanjut untuk menjamin kualitas data yang akan dilatih.
- Terdapat indikasi data outlier pada fitur Pregnancies, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction. Hal ini perlu ditangani lebih lanjut untuk menjaga performa model prediksi yang dihasilkan nantinya.

#### 2. Korelasi Antar Fitur
<img width="520" alt="3_correlation-heatmap" src="https://github.com/user-attachments/assets/072b5cbe-8935-4c3b-9c19-a92ef78db2c6" />

**Hasil analisis heatmap correlation:**
*   Kadar glukosa menunjukkan pengaruh yang tertinggi terhadap outcome dibandingkan dengan fitur lainnya. Korelasi positif cukup kuat, artinya semakin tinggi kadar glukosa maka semakin besar kemungkinan diabetes.
*  Jumlah produksi Insulin dan skin thickness menunjukkan korelasi positif yang moderat. sehingga orang dengan insulin tinggi cenderung memiliki ketebalan kulit yang lebih besar.
*   Pregnancies dan Age memiliki korelasi positif yang cukup kuat yang menunjukkan semakin tua, semakin banyak kehamilan biasanya.
*  Secara keseluruhan tidak terdapat korelasi fitur yang sangat tinggi (>0.75) sehingga tidak perlu melakukan drop fitur karena multikolinearitas.

#### 3. Eksplore Keberadaan Outlier di setiap Fitur
<img width="935" alt="4_box-plot-outlier" src="https://github.com/user-attachments/assets/7a62b7c7-813e-4204-95c0-02608013cd72" />

**Analisis boxplot:**
*   Fitur Pregnancies memiliki beberapa outlier diatas yang bernilai >13.
*   Fitur Glucose memiliki outlier dengan nilai ekstrem (0), kemungkinan nilai ini tidak valid.
*   Fitur BloodPreasure memiliki beberapa outlier  dibawah dengan nilai ekstream mencapai 0, ini tidak masuk akal dan mengindikasikan invalid value.
*   Fitur Skin Thickness memiliki outlier dengan nilai yang sangat tinggi.
*   Fitur Insulin memiliki sangat banyak data outlier dengan nilai yang sangat tinggi
*   Fitur BMI memiliki cukup banyak outlier dengan nilai yang sangat tinggi dan terdapat juga outlier dengan nilai sangat kecil yaitu 0 yang kemungkinan merupakan invalid value.
*   Fitur DiabetesPredigreeFunction memiliki sangat banyak data outlier dengan nilai yang tinggi
*   Fitur Age memiliki beberapa outlier dengan nilai yang tinggi.

#### 4. Eksplor Proporsi Outcome
<img width="349" alt="5_outcome-distribution" src="https://github.com/user-attachments/assets/e1300350-58a5-4fc2-9c43-b7b4bac08fb0" />

**Analisis Grafik Distribusi Outcome Diabetes:**
Data dengan outcome 0 (tidak menderita diabetes hampir 2 kali lebih banyak dibandingkan dengan outcome bernilai 1 (menderita diabetes).
Hal ini bisa berpengaruh pada saat proses pelatihan dimana model lebih hafal dengan data yang dominan dan gagal memprediksi data minoritas.
Sehingga, diperlukan penanganan untuk menyeimbangkan proporsi data atau pemilihan algoritma yang yang tahan akan imbalance data.
**Solusi:** Resampling data dengan melakukan Oversampling maupun Undersampling untuk menyeimbangkan  jumlah data di kedua outcome.

## Data Preparation
Tahap data preparation bertujuan untuk mempersiapkan data yang bersih dan siap untuk dilatih. Tahapan data preparation meliputi penanganan invalid data, penaganan outlier, penanganan imbalance data, dan data splitting.
#### 1. Penanganan Invalid Data
Penanganan invalid data dilakukan agar setiap fitur memiliki data yang masuk akal dan sesuai dengan keadaan di dunia nyata. Hampir di keseluruhan fitur terdapat nilai yang tidak valid sehingga perlu untuk ditangani agar tidak mempengaruhi hasil prediksi model yang akan dilatih. Teknik yang digunakan untuk menanganani invalid value adalah drop (menghapus data yang tidak valid) dan imputasi (mengganti data yang tidak valid dengna sebuah nilai yang lebih valid). Pemilihan teknik yang diterapkan bergantung pada beberapa pertimbangan seperti jumlah data yang valid, jika invalid data sedikit maka dapat dilakukan drop. Sebaliknya, jika data yang invalid cukup banyak sebaiknya dilakukan imputasi agar tidak kehilangan terlalu banyak data untuk dilatih. Berikut adalah langkah penganganan invalid data:
1. Fitur `Glucose` memiliki 5 buah data yang tidak valid, sehingga dilakukan tindakan drop data.
2. Fitur `BMI` memiliki 11 data yang tidak valid, sehingga dilakukan tindakan drop data.
3. Fitur `BloodPressure` memiliki 28 buah data tidak valid, sehingga dilakukan tindakan drop data.
4. Fitur `SkinThickness` memiliki 192 buah data tidak valid. Jumlah data invalid cukup banyak sehingga dilakukan imputasi dengan nilai median.
5. Fitur `Insulin` memiliki 332 buah data yang tidak valid. Jumlah data invalid cukup banyak sehingga dilakukan imputasi dengan nilai median.

#### 2. Penanganan Outlier 
Penanganan Outlier dilakukan dengan hati-hati agar tidak merusak variasi data dan menghilangkan pola dalam data. Penanganan outlier pada data dengan outlier sedikit dikenakan metode drop (menghapus data outlier langsung, sedangkan fitur dengan jumlah outlier yang cukup banyak dikenakan teknik imputasi nilai median tanpa outlier yang diperoleh dengan Metode IQR. Berikut adalah langkah penanganan outlier:
1. Fitur `Pregnancies` memiliki 4 data outlier dengan angka yang cukup besar uangk jumlah kehamilan seseorang. Penganganan yang dilakukan terhadap fitur ini adalah drop data.
2. Fitur `BloodPressure`, `SkinThickness`, `Insulin`, `BMI`, memiliki cukup banyak data outlier sehingga dilakukan imputasi dengan nilai `lower_bound` dan `upper_bound` masing-masing fitur tersebut.

Berikut merupakan hasil akhir dari penanganan outlier pada beberapa fitur.
<img width="637" alt="6_box-plot-outlier-clean" src="https://github.com/user-attachments/assets/63a3f80e-5c5c-47eb-9a82-9e8f98e4860c" />

#### 3. Penanganan Data Imbalance
Distribusi Outcome menunjukkan imbalance data dimana data bernilai 0 (tidak mengidap diabetes) berjumlah hampir 2 kali lipat dari data lainnya. Maka, akan dilakukan Resampling terhadap data minoritas agar menghasilkan jumlah data yang seimbang di setiap outcome. Metode yang digunakan adalah SMOTE (Synthetic Minority Over-sampling Technique). Dengan metode ini akan menghasilkan data baru pada kelas minoritas yaitu outcome = 1 tanpa mengubah variasi atau informasi pada data asli.
Sehingga diperoleh hasil resampling data dengan metode SMOTE sebagai berikut:

<img width="368" alt="7_outcome-distribution-balanced" src="https://github.com/user-attachments/assets/d46d9f63-c110-4880-8c45-9f476ffd6bdf" />

#### 4. Data Splitting
Data Splitting adalah proses membagi dataset menjadi dua bagian utama yaitu data pelatihan (training) dan data pengujian (testing). Dalam proyek ini, pembagian data dilakukan dengan perbandingan 80% untuk pelatihan dan 20% untuk pengujian. Data yang telah dilakukan resampling kini berjumlah 950sehingga akan dibagi dan dicobakan pada setiap algoritma juga dengan 760 sampel data latih dan 190 sampel data uji. Berikut kerangka kode program yang digunakan:

    #kode program
    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

## Modeling
Pada tahap modeling, akan dilakukan pengembangan model machine learning dengan tiga algoritma, yang antara lain:

**1. SVM**
SVM bekerja dengan mencari hyperplane yang optimal untuk memisahkan data ke dalam kelas-kelas yang berbeda. Hyperplane adalah garis (pada data dua dimensi) atau bidang (pada data tiga dimensi) yang memisahkan data dari kelas berbeda. Tujuan SVM adalah menemukan hyperplane yang memaksimalkan margin, yaitu jarak antara hyperplane dan titik data terdekat dari setiap kelas.

Dalam algoritma SVM, beberapa parameter utama perlu diatur untuk mengoptimalkan performa model. Inilah beberapa parameter yang digunakan dalam projek ini:
- `Kernel=rbf`: Menentukan jenis fungsi kernel yang digunakan. `rbf` atau Radial Basic Function cocok untuk data non-linear.
- `probability=True`: Mengaktifkan perhitungan probabilitas untuk hasil prediksi.
- `random_state=55`: Menetapkan nilai acak yang tetap (fixed seed) agar proses pelatihan menjadi reproducible, artinya hasil pelatihan akan selalu sama jika kode dijalankan ulang.
        
Alasan pemilihan algoritma SVM adalah karena algoritma ini efektif untuk data berdimensi tinggi, cocok untuk klasifikasi biner seperti prediksi diabetes, dan mampu memaksimalkan kela dengan margin yang maksimal.
Akan tetapi algoritma ini memiliki kelemahan seperti memerlukan waktu komputasi yang besar pada dataset yang besar dan sensitif terhadap skala fitur.

**2. Boosting Algorithm (Adaptive Boosting)**
Algoritma Boosting bertujuan untuk meningkatkan performa atau akurasi prediksi. Caranya adalah dengan menggabungkan beberapa model sederhana dan dianggap lemah (weak learners) sehingga membentuk suatu model yang kuat (strong ensemble learner).
Dilihat dari caranya memperbaiki kesalahan pada model sebelumnya, algoritma boosting terdiri dari dua metode:
        - Adaptive boosting
        - Gradient boosting

Pada proyek ini akan menggunakan metode Adaptive Boosting yang terkenal yaitu AdaBoost. Berikut merupakan parameter-parameter yang digunakan pada proyek ini:
- `learning_rate=0.05`: untuk mengontrol kontribusi tiap estimator, semakin kecil nilai maka model belajar semakit lambat dan lebih konservatif.
- `random_state=55`: Menetapkan nilai acak yang tetap (fixed seed) agar proses pelatihan menjadi reproducible, artinya hasil pelatihan akan selalu sama jika kode dijalankan ulang.
    
Alasan penggunaan algoritma AdaBoost adalah kemampuannya untuk meningkatkan akurasi model dengan penggabungan beberapa model, tahan terhadap overfitting jika dilakukan konfigurasi yang pas, dan performa cukup bagus untuk data kompleks dan tidak linear.
Akan tetapi algoritma ini memiliki kelemahan seperti rentan terhadap outlier dan waktu pelatihan bisa lebih lama dibandingkan algoritma lainnya.

**3. Logistic Regression**
Logistic Regression adalah salah satu algoritma klasifikasi yang digunakan untuk memprediksi probabilitas dari sebuah input termasuk ke dalam salah satu dari dua kelas (misalnya: "positif diabetes" atau "negatif diabetes"). Meskipun namanya "regression", algoritma ini bukan untuk prediksi nilai kontinu, melainkan digunakan untuk memecahkan masalah klasifikasi biner.Parameter SVM yang digunakan pada proyek ini:
- `random_state=55`: Menetapkan nilai acak yang tetap (fixed seed) agar proses pelatihan menjadi reproducible, artinya hasil pelatihan akan selalu sama jika kode dijalankan ulang.

Alasan pemilihan algoritma ini adalah karena algoritma ini sederhana dan cepat dilatih. Selain itu Logistic Regression mudah diinterpretasikan.
Akan tetapi algoritma ini memiliki kelemahan seperti tidak mampu menangkap pola pada fitur dengan hubungan non-linear secara langsung.

Setelah melakukan pelatihan dengan ketiga algoritma tersebut, diperoleh model-model machine learning yang dapat digunakan untuk melakukan prediksi penyakit diabetes. Setiap Algoritma menghasilkan performa yang berbeda-beda sehingga dapat dipilih salah satu model dengan performa terbaik. Berdasarkan akurasi setiap algoritma memperoleh akurasi sebagai berikut:
- SVM Accuracy: 0.7474
- AdaBoost Accuracy: 0.8316
- Logistic Regression Accuracy: 0.7368

Dan Confusion Matrix sebagai berikut:
![8_confussion-matrix](https://github.com/user-attachments/assets/4980637b-4b2d-4d4e-a9a1-20842dd57526)

Dari hasil yang diberikan model yang dilatih dengan AdaBoost memiliki jumlah prediksi benar lebih banyak di setiap kelas dibandingkan model lainnya. Untuk evaluasi lebih lanjut terhadap model terdapat pada bagian evaluation.

## Evaluation
Tahap evaluasi dilakukan dengan menggunakan beberapa metrik pengukuran seperti Accuracy, Precision, Recall, F1-Score, dan AUC. Berikut penjelasan dari masing-masing metrik:
**1. Accuracy**
Akurasi adalah metrik yang paling sederhana dan sering digunakan untuk mengukur kinerja model klasifikasi. Akurasi dihitung sebagai proporsi dari prediksi benar (baik positif maupun negatif) terhadap seluruh prediksi yang dilakukan oleh model.
![Dicoding-Acuracy](https://assets.cdn.dicoding.com/original/academy/dos-701b28b93cb6ba8c3e9d6b9c8c1bae9920241015153232.jpeg)
Contoh: Jika model Anda membuat 100 prediksi dan 90 di antaranya benar (baik positif maupun negatif), akurasi model tersebut adalah 90%. Namun, akurasi bisa menyesatkan jika ada ketidakseimbangan kelas (misalnya, jika ada banyak lebih banyak contoh dari satu kelas dibandingkan dengan kelas lainnya).

**2. Precision**
Precision mengukur seberapa baik model menghindari positif palsu (false positives, FP). Ini adalah rasio prediksi positif yang benar terhadap semua prediksi positif yang dibuat oleh model.
![Dicoding-Precision](https://assets.cdn.dicoding.com/original/academy/dos-fc5f282672f1b572c4cd9a0e747dec5e20241015153231.jpeg)
Contoh: Dalam sebuah model yang digunakan untuk mendeteksi diabetes, presisi tinggi berarti bahwa sebagian besar dari data yang diklasifikasikan sebagai penderita diabetes benar-benar merupakan penderita diabetes, dan sangat sedikit transaksi yang tidak menderita diabetes diklasifikasikan secara salah sebagai penderita diabetes

**3. Recall**
Recall atau sensitivitas adalah metrik yang mengukur seberapa baik model dapat menangkap semua contoh positif. Ini adalah rasio prediksi positif yang benar terhadap semua kasus positif yang sebenarnya ada dalam data.
![Dicoding-Recall](https://assets.cdn.dicoding.com/original/academy/dos-d17ca76e6a72ddc98ed5c803561cf20820241015153231.jpeg)
Contoh: Dalam konteks prediksi diabetes, recall yang tinggi berarti model mampu mendeteksi sebagian besar dari semua kasus diabetes yang ada sehingga mengurangi risiko terlewatnya diagnosis.
    
**4. F1-Score**
F1-Score adalah metrik yang menggabungkan presisi dan recall menjadi satu nilai tunggal yang mempertimbangkan keduanya. F1-Score adalah rata-rata harmonis dari presisi dan recall, memberikan gambaran yang lebih baik ketika ada trade-off antara keduanya.
![Dicoding-F1-Score](https://assets.cdn.dicoding.com/original/academy/dos-0ab2c6bcc31494e4c1cc70008ae9a31620241015153232.jpeg)
Contoh: F1-Score berguna dalam situasi jika ada ketidakseimbangan antara kelas positif dan negatif. Jika model memiliki presisi dan recall yang tidak seimbang, F1-Score dapat memberikan gambaran lebih akurat tentang performa keseluruhan model.

**5. AUC**
AUC (Area Under the Curve) adalah luas di bawah kurva ROC (Receiver Operating Characteristic). Kurva ROC menggambarkan seberapa baik model machine learning dapat membedakan kedua kelas yang ada pada data diabetes. Semakin besar nilai AUC maka semakin baik model dalam membedakan kelas.
Kurva ROC dibentuk dengan cara sebagai berikut:
- Sumbu X: menunjukkan False Positive Rate (FPR) → berapa banyak yang seharusnya negatif, tapi diprediksi positif.
- Sumbu Y: menunjukkan True Positive Rate (TPR) atau Recall → berapa banyak yang seharusnya positif dan berhasil diprediksi dengan benar.
    
Lalu, AUC menghitung luas di bawah kurva tersebut. Nilainya antara 0 dan 1:
    - AUC = 1 → model sempurna.
    - AUC = 0.5 → model seburuk menebak acak.
    - AUC < 0.5 → model sangat buruk,

Contoh sederhananya, misalnya terdapat 100 orang pasien. Model yang dibangun menghasilkan prediksi dalam bentuk probabilitas, kemudian dilakukan evaluasi untuk melihat sejauh mana model mampu memberikan skor yang lebih tinggi kepada pasien yang benar-benar mengidap penyakit dibandingkan dengan yang tidak.
Apabila seluruh pasien yang mengidap penyakit memperoleh skor lebih tinggi dibandingkan pasien yang sehat, maka nilai AUC adalah 1 (sempurna). Sebaliknya, jika prediksi model tidak konsisten—ada kalanya benar, ada kalanya salah—maka nilai AUC dapat berada di kisaran 0,7.
    
**Analisis Evaluasi Hasil Proyek:**

<img width="512" alt="9_evaluation-metric" src="https://github.com/user-attachments/assets/285d6ff4-fa29-41b5-99a1-ed438e290f0d" />

**1. SVM**
- Accuracy model sebesar 0.747368 menunjukkan model berhasil memprediksikan dengan benar sebesar 74% dari total data.
- Precision sebesar 0.771084, berarti model bisa memprediksi apakah mengidap diabetes dengan kemungkinan cukup besar bahwa hasil prediksi benar.
- Recall hanya mencapai 0.6882, berarti banyak kasus diabetes yang salah prediksi.
- F1-Score menunjukkan keseimbangan antara precision dan recall model mencapai 0.727273
- AUC cukup tinggi yaitu 0.863541, ini menunjukkan model cukup baik dalam membedakan kelas 0 dan 1.
- ModelSVM yang dihasilkan cukup mampu membedakan kelas namun cenderung melewatkan kasus diabetes terlihat dari kasus kesalahan prediksi kasus diabetes menjadi tidak diabetes.

**2. Boosting Algorithm (AdaBoostClassifier)**
- Accuracy mencapai 0.831579, berarti model mampu memprediksi 83,2% data dari keseluruhan data dengan benar.
- Precision cukup tinggi yaitu 0.808081, berarti model mungkin benar memprediksikan kasus pengidap diabetes dengan benar cukup tinggi.
- Recall mencapai 0.860215, berarti model mampu mengidentifikasi sekitar 86.0% dari semua kasus diabetes.
- F1-Score mencapai 0.833333, menunjukkan precision dan recall cukup seimbang.
- AUC mencapai 0.881665, berarti model cukup baik dalam membedakan kelas.
- kinerja cukup baik di semua metrik, Recall dan F1-Score yang cukup tinggi menunjukkan kemampuan model yang baik dalam prediksi setiap kelas.

**3. Logistic Regression**
- Akurasi sebesar 0.736842, merupakan yang terkecil dari model lainnya.
-  Precision bernilai 0.736264 cukup rendah dibandingkan model svm dan adaboost.
- Recall mencapai 0.720430 lebih tinggi dari pada model svm, ini berarti model lebih mampu memprediksi kasus diabetes dengan benar dibanding model svm, namun nilai ini cukup baik.
- F1-Score mencapai 0.728261, artinya keseimbangan precision dan recall masih mencapai 72%.
- AUC mencapai 0.804900, model ini cukup dalam membedakan dua kelas.
- Performa rata-rata di semua metrik, tidak terlalu baik tapi kalah dari modeal svm dan adaboost.

📑 Rangkuman Evaluasi:
    **Akurasi Tertinggi**: AdaBoost
    **Recall Tertinggi**: AdaBoost
    **AUC Tertinggi**: AdaBoost
    **Precision Tertinggi**: AdaBoost
    **F1-Score Tertinggi**: AdaBoost

✨ Model Terbaik: 
    **AdaBoost** merupakan model terbaik untuk tugas klasifikasi prediksi diabetes dibandingkan model yang telah dihasilkan lainnya karena performanya yang stabil dan konsisten

---
# Kesimpulan
Telah dilakukan eksplorasi terhadap seluruh fitur pada dataset. Semua fitur digunakan dalam proses pelatihan karena tidak ditemukan ketergantungan antar fitur, dan masing-masing fitur menunjukkan pola yang relevan.

Dataset telah dianalisis dan ditemukan beberapa permasalahan seperti data tidak valid, outlier, serta ketidakseimbangan kelas (imbalanced data). Masalah tersebut telah ditangani menggunakan teknik yang sesuai dengan karakteristik dataset.

Model machine learning telah dilatih menggunakan beberapa algoritma, yaitu SVM, AdaBoost, dan Logistic Regression, untuk memprediksi apakah seseorang mengidap diabetes berdasarkan data pemeriksaan medis.

Evaluasi dilakukan menggunakan metrik Accuracy, Precision, Recall, F1-Score, dan AUC. Hasil evaluasi menunjukkan bahwa model AdaBoost memberikan performa terbaik secara keseluruhan, dengan nilai yang lebih tinggi dan konsisten di setiap metrik dibandingkan algoritma lainnya.

Terima Kasih
