# Mengurangi Tiket Pending: Analisis Kategori Masalah dan Waktu Penyelesaian

## Repository Outline
Pada repository ini file yang saya push ada 3 file, yaitu :

1. description.md
2. P0M1_Angga.ipynb
3. P0M1_Angga_dataset.csv
4. P0M1_Angga_dataset_Data_Asli.csv

## Problem Background
Specific : menangani tiket dukungan teknis dengan lebih efisien, terutama pada mengurangi waktu penyelesaian yang memakan waktu terlalu lama dan kepuasan dari sisi user.

Measurable : meningkatkan persentase penyelesaian case user dalam waktu kurang dari 60 menit dan mengurangi jumlah status pending menjadi 10%.

Achievable : melatih tim support dengan Solusi yang lebih efektif dan efisien dalam waktu penyelesaian.

Relevant : meningkatkan efisiensi penyelesaian tiket dan kepuasan user, dan mengurangi beban kerja tim support.

Time-Bound : Target terealisasi dalam 3 bulan.

**Ringkasan Problem statement**
bagaimana mengurangi waktu penyelesaian case dengan meningkatkan persentase penyelesaian dan mengurangi jumlah status pending sebesar 10% dengan melatih tim support untuk meningkatkan kepuasan user dan mengurangi beban kerja tim support dalam kurun waktu 3 bulan.

references Measurable: https://www.endsight.net/blog/it-support-help-desk-metrics-and-benchmarks

## Project Output
Dari analisis yang telah saya lakukan terhadap dataset diatas adalah analisis statistik waktu rata - rata untuk menyelesaikan tiket adalah 63 menit, dan tidak ada hubungan yang kuat antara Issue_Category dan Issue_Status. Pada visualisasi data distribusi Issue_Customer masalah yang paling sering dialami user, yaitu *Slow System Performance* dengan 293 tiket yang ada pada dataset. Selain itu, pada kategori masalah jaringan memiliki waktu penyelesaian yang paling lama, yaitu 65 menit. dari distribusi tiket, ditemukan bahwa terdapat selisih antara tiket yang berstatus pending dan yang telah resolved hanya 1.8%. Dan yang terakhir kategori hardware yang memiliki jumlah tiket pending terbanyak, yaitu sebanyak 402 tiket.

Kesimpulannya meskipun tidak adanya hubungan yang signifikan antara kategori masalah dan status tiket, beberapa kategory tertentu menunjukkan waktu penyelesaian lebih lama dan jumlah tiket yang berstatus pending lebih tinggi, yang dapat menjadi perhatian untuk perbaikan sistem atau membuat SOP yang lebih ketat lagi untuk Tim IT Ssupport.

## Data 
Data yang saya gunakan untuk melakukan analisys ini adalah data yang bersumber dari kaggle, pada dataset ini terdapat jumlah column sebanyak 6 column, lalu untuk baris data sebanyak 1.896, untuk data yang saya gunakan ini adalah data yang telah bersih.

## Method
Pada project ini saya menggunakan beberapa metode untuk melakukan analisys ini seperti, berikut :
1. Analisys Statistic Deskriptif.
2. Analisys Statistic Inferencial pada analisys ini saya menggunakan metode hipotesis dengan uji Chi-Squared dengan conviden level 95%.
3. Saya melakukan analisys dengan visualisasi.

## Stacks
import pandas as pd
import numpy as np

import seaborn as sns
import matplotlib.pyplot as plt
import plotly.express as px

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
from scipy import stats

from matplotlib.gridspec import GridSpec

## Reference
Link dataset : https://www.kaggle.com/datasets/steve1215rogg/tech-support-conversations-dataset?resource=download

Link Dasboard : https://public.tableau.com/views/DasboardAnalisisVisualisasiStatisticTiketITSupport/DashboardAnalisysVisual?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

references Measurable: https://www.endsight.net/blog/it-support-help-desk-metrics-and-benchmarks