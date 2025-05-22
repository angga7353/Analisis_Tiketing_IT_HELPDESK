# Analisis_Tiketing_IT_HELPDESK
##Link Dataset dan Link Dashboard
[DataSet](https://www.kaggle.com/datasets/steve1215rogg/tech-support-conversations-dataset?resource=download)
[Dasboard](https://public.tableau.com/views/DasboardAnalisisVisualisasiStatisticTiketITSupport/DashboardAnalisysVisual?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

# Tujuan Project
Proyek ini bertujuan untuk mengurangi waktu penyelesaian kasus (case resolution time) secara signifikan dengan pendekatan yang terukur dan berfokus pada pengembangan tim support. Sasaran utama yang ingin dicapai dalam kurun waktu 3 bulan adalah:
* Meningkatkan persentase penyelesaian kasus secara keseluruhan untuk memastikan lebih banyak kasus yang ditangani dapat diselesaikan dengan cepat dan efektif.
* Mengurangi jumlah kasus dengan status pending sebesar 10%, sehingga meminimalisir keterlambatan dan menurunkan backlog yang menghambat produktivitas.
* Melalui program pelatihan intensif bagi tim support, diharapkan tim dapat:
  * Meningkatkan kepuasan pengguna (user satisfaction) dengan memberikan solusi yang lebih tepat dan responsif.
  * Mengurangi beban kerja tim support melalui peningkatan efisiensi proses kerja, pengelolaan kasus yang lebih baik, dan penerapan teknik troubleshooting yang lebih      efektif.
Dengan target ini, proyek diharapkan dapat memberikan dampak positif yang nyata pada kinerja tim support dan pengalaman pengguna secara keseluruhan.

# Hasil Analisis
Berdasarkan analisis statistik yang telah dilakukan terhadap dataset di atas, berikut adalah temuan utama yang diperoleh:
* Rata-rata waktu penyelesaian tiket adalah sekitar 63 menit.
* Tidak ditemukan hubungan yang kuat antara variabel Issue_Category dan Issue_Status, yang berarti kategori masalah tidak secara signifikan mempengaruhi status tiket.
* Dari visualisasi distribusi data pada variabel Issue_Customer, masalah yang paling sering dialami oleh pengguna adalah Slow System Performance, dengan total 293 tiket yang tercatat dalam dataset.
* Pada kategori masalah jaringan, ditemukan bahwa waktu penyelesaian rata-rata merupakan yang paling lama, yaitu 65 menit, menunjukkan perlunya perhatian khusus pada masalah jaringan.
* Dari distribusi tiket, ditemukan selisih yang sangat kecil yaitu hanya 1.8% antara jumlah tiket berstatus pending dan yang telah resolved, yang mengindikasikan bahwa hampir semua tiket berprogres dengan baik.
* Terakhir, kategori hardware memiliki jumlah tiket berstatus pending terbanyak, yakni sebanyak 402 tiket, yang menjadi titik perhatian khusus dalam pengelolaan kasus.
## Kesimpulan
Meskipun analisis tidak menunjukkan adanya hubungan signifikan antara kategori masalah dan status tiket, beberapa kategori tertentu seperti masalah jaringan dan hardware menunjukkan:
* Waktu penyelesaian yang lebih lama,
* Jumlah tiket pending yang lebih tinggi.
Hal ini menunjukkan perlunya perhatian lebih pada kategori tersebut, baik melalui perbaikan sistem maupun pengembangan Standard Operating Procedure (SOP) yang lebih ketat dan terstruktur untuk Tim IT Support guna meningkatkan efektivitas penanganan tiket dan kepuasan pengguna.

# Sumber dan Deskripsi Data
Data yang digunakan untuk melakukan analisis ini bersumber dari Kaggle, sebuah platform penyedia dataset publik yang terpercaya.
* Dataset terdiri dari 6 kolom yang merepresentasikan berbagai atribut terkait tiket masalah (issue tickets).
* Jumlah baris data dalam dataset adalah 1.896 entri.
* Data yang digunakan sudah melalui proses pembersihan (cleaning) sehingga siap untuk dianalisis tanpa adanya nilai yang hilang atau data tidak valid.
Dengan data yang sudah bersih ini, analisis statistik dan visualisasi dapat dilakukan secara akurat dan memberikan hasil yang dapat diandalkan untuk pengambilan keputusan.

# Library dan Tools yang Digunakan
Dalam analisis data yang dilakukan, saya menggunakan beberapa library Python utama sebagai berikut:
* pandas dan numpy: Untuk manipulasi data dan operasi numerik yang efisien.
* seaborn dan matplotlib.pyplot: Untuk visualisasi data statistik dengan grafik yang informatif dan estetis.
* scipy.stats: Untuk analisis statistik lanjutan seperti pengujian hipotesis.
Penggunaan library tersebut memungkinkan pengolahan data yang efektif, serta visualisasi yang membantu dalam interpretasi hasil analisis. 
