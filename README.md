
# NYC TLC Taxi Data Analysis  
## *Operational Efficiency & Route Optimization*  
### Capstone Project Modul 2 — Fajar Hafizhuddin

Proyek ini menganalisis dataset perjalanan taksi dari **New York City Taxi & Limousine Commission (TLC)** untuk memahami efisiensi operasional, mengidentifikasi rute tidak efisien, serta memberikan rekomendasi optimasi berbasis data.


---

## 1. Business Understanding

### **Business Context**  
NYC Taxi beroperasi dalam lingkungan urban yang padat dan dinamis. Perjalanan taksi dipengaruhi oleh:

- Kemacetan  
- Waktu penjemputan  
- Lokasi pickup & dropoff  
- Struktur tarif  
- Pola pergerakan penduduk  

Efisiensi perjalanan sangat penting karena memengaruhi **profit perusahaan**, **pendapatan pengemudi**, dan **kepuasan penumpang**.

---

### **Business Stakeholders**
- NYC Taxi Companies  
- Fleet & Operations Managers  
- Taxi Drivers  
- NYC TLC (Regulator)  
- Customers  
- Data Analysts  

---

### **Problem Statement**
- Rute mana yang **paling tidak efisien**?  
- Faktor apa yang memengaruhi efisiensi?  
- Zona mana yang padat tetapi performanya rendah?  
- Jam berapa efisiensi menurun secara signifikan?  
- Bagaimana armada dapat dialokasikan secara optimal?  

---

## 2. Data Understanding

### **Sumber Data**
Data publik dari New York City Taxi & Limousine Commission (TLC)

---

### **Struktur Kolom Dataset**

#### **Trip Information**
- lpep_pickup_datetime  
- lpep_dropoff_datetime  
- trip_distance  
- duration_min / duration_hr  
- speed_mph  

#### **Location Identifiers**
- PULocationID  
- DOLocationID  
- RatecodeID  

#### **Passenger & Trip Attributes**
- passenger_count  
- payment_type  
- trip_type  

#### **Fare & Revenue Components**
- fare_amount  
- tip_amount  
- tolls_amount  
- total_amount  
- congestion_surcharge  

#### **Derived Metrics**
- cost_per_mile  
- cost_per_min  
- efficiency_index  

---

## 3. Data Cleaning

- Menghapus missing values  
- Parsing datetime  
- Menghitung durasi & kecepatan  
- Menghapus trip tidak valid  
- Membuat variabel turunan seperti efficiency_index  

---

## 4. Exploratory Data Analysis (EDA)

- Efisiensi Berdasarkan Jarak, Durasi, dan Kecepatan
- Distribusi berdasarkan distance, duration, cost, and speed 
- Top 10 Pickup Zones by number of trips 
- Perbandingan Jarak dan Harga

---

## 5. Diagnostic Analysis

### **Rute Tidak Efisien**
- Kecepatan rendah  
- Durasi panjang  
- Volume tinggi tetapi efisiensi rendah  

### **Efisiensi Perjalanan Berdasarkan Waktu**
- Rush hours: 07–10 & 16–19 → efisiensi turun  
- Night hours lebih efisien  

### **Total Pendapatan Berdasarkan zona penjemputan dan Jenis Pembayaran**
- Credit card > 70% revenue  
- Zona tertentu high revenue tetapi low efficiency  

---

## 6. Conclusion

* Efisiensi dipengaruhi oleh jarak, durasi, dan kepadatan lalu lintas.
* Rute dengan banyak perjalanan dapat tetap tidak efisien jika kecepatan rata-rata rendah.
* Efisiensi menurun pada morning dan evening rush hour.
* Efisiensi meningkat pada malam hingga dini hari.
* Zona dengan revenue tinggi tidak selalu yang paling banyak trip-nya.
* Pembayaran menggunakan kartu mendominasi pendapatan.
* Ada peluang besar untuk perbaikan melalui optimasi rute dan strategi operasional.
---

## 7. Recommendations

* Optimalkan alokasi armada ke zona demand tinggi & efisiensi baik.
* Pertimbangkan penggunaan jalur alternatif untuk zona padat.
* Perkuat distribusi armada di zona yang memberikan revenue tinggi.
* Analisis ulang tarif di zona volume tinggi tetapi pendapatan rendah.
* Gunakan pola efisiensi per jam untuk penjadwalan armada yang lebih optimal.

---

## 8. License
Data oleh **NYC Taxi & Limousine Commission (TLC)**.  
