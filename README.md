# Data Science Project 1 : Estimasi Harga Laptop Gaming
# *by Jevis Xandra*

## Pendahuluan
![Value vs Price](https://media.licdn.com/dms/image/C5612AQGwU4rFPyen0w/article-cover_image-shrink_600_2000/0/1520169366642?e=2147483647&v=beta&t=3tRN_EwJplmeVbvMnn9zuv8dSqgkF79aqG8TPtadPJA)

Saya percaya teman-teman yang ada di sini pernah mengalami pengalaman seperti ini. Suatu hari, teman-teman sedang berjalan ke mall atau supermarket untuk membeli charger smartphone karena charger smartphone teman-teman yang sebelumnya sudah rusak. Tapi ini merupakan kali pertama teman-teman membeli charger smartphone dan tidak tahu harga nya karena charger yang sebelumnya sudah diberikan sepaket dengan smartphone ketika teman-teman membeli smartphone nya. Tentu saja di sini sebelum membeli, teman-teman membutuhkan beberapa info sebagai referensi atau pertimbangan, misalkan : berapa sih daya listrik charger yang cocok untuk smartphone saya? atau berapa pula harga yang normal untuk charger smartphone seperti ini?. Mungkin teman-teman akan menanyakan hal tersebut ke teman yang sudah berpengalaman atau mencari informasi tersebut lewat google dan lain sebagai nya. Tujuan nya supaya teman-teman tidak membeli cahrger yang kemahalan atau kemurahan (yang ada kemungkinan merupakan barang rusak). Berangkat dari pengalaman umum seperti itu, saya menjadi terinspirasi untuk membangun sebuah program kecil atau model yang dapat mengestimasi harga suatu barang berdasarkan spesifikasi yang kita masukkan ke program tersebut. Di proyek ini saya akan membuat suatu model yang mengestimasi harga laptop gaming berdasarkan spesifikasi yang dimasukkan.

## Garis Besar Proyek
Pada proyek kali ini, ada beberapa tahapan yang saya lakukan mulai dari pengumpulan data hingga pembuatan model :
* **Data mining** menggunakan python dengan modul Selenium dan BeautifulSoup melalui salah satu website penjualan peralatan elektronik dari India "www.smartprix.com"
* **Data Cleaning** dan **Data Wrangling** laptop gaming mentah yang di-scrap melalui website tersebut yang mencakup penghapusan kolom tertentu, mengganti format/datatype kolom, dan mengisi data yang hilang
* **Data Exploration** untuk menentukan parameter yang akan dijadikan prediktor. Tentu saja parameter yang dipilih diharapkan memiliki korelasi yang cukup kuat dengan harga laptop gaming.
* **Training dan Validate Model** regresi linear yang performansi nya paling bagus dan membuat model tersebut berdasarkan keseluruhan data yang ada.

## Kesimpulan 
* Di antara data numerik dan data kategori yang format nya bilangan bulan (integer), "**Solid State Drive**" merupakan parameter yang memiliki korelasi paling tinggi dengan harga sebuah laptop gaming.
* Beberapa data kategori yang format nya teks (string) yang berkorelasi kuat dengan harga laptop gaming, antara lain : **Resolution**, **RAM**, **OS Version**, **Processor**.
* Model yang memberikan performansi paling bagus di antara model yang dicoba adalah **Artificial Neural Network Regression Model**.
