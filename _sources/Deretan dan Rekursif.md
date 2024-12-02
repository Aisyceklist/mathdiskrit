---
title: Deretan dan Rekursif

---

# Deretan dan Rekursif
## Deretan
### Pengertian
Deretan adalah suatu urutan elemen atau objek yang susun secara teratur berdasarkan suatu aturan tertentu . Elemen dalam deretan biasanya berupa angka, huruf, simbol atau objek lainnya. dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu.

Definisi: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.

N = {1, 2, 3, 4, … } S misalnya {2, 4, 6, 8, …}, {1/3, 1/5, 1/7, …}, dsb

Notasi deretan: {$a_n$}

Deretan umumnya dinyatakan dalam suatu formula, misalnya: 
$a_n$ = 2n 
$a_n$ = 1/n 
$a_n$ = 7 – 3n

Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu. Misalnya:
1. Deretan bilangan ganjil: 1,3,5,7,…
2. Deretan bilangan genap: 2,4,6,8,
3. Deretan bilangan yang membentuk deret aritmetika: 3,6,9,12….

### Contoh-contoh deretan dan formulanya
#### Deret Aritmetika
Deret dengan pola kenaikan atau penurunan tetap.

Contoh: 2,5,8,11,14,…
Rumus suku ke-n: $U_n = a + (n - 1) \cdot b$
dimana:
𝑎: suku pertama 
𝑏: beda (selisih antar suku 𝑛: nomor suku yang dicari


#### Deret Geometri
Deret dengan pola kelipatan tetap.

Contoh: 3,6,12,24,48,…
Rumus suku ke-n: $U_n = a \cdot r^{(n-1)}$
    Dimana : 
    𝑎: suku pertama 
    𝑟: rasio (perbandingan antar suku
    𝑛: nomor suku yang dicari
    
#### deret Bilangan Kuadrat
Deret dengan pola nilai berupa kuadrat bilangan bulat.

Contoh: 1,4,9,16,25,…
Rumus suku ke-n: $u_n=n^2$

#### Deret Bilangan Kubik
Deret dengan pola nilai berupa kubik bilangan bulat.

Contoh: 1,8,27,64,125,…
Rumus suku ke-n:  $u_n=n^3$

#### Deret Fibonacci
Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.

Contoh: 0,1,1,2,3,5,8,…
Rumus suku ke -n (rekursif): $𝐹_𝑛=𝐹_{(𝑛−1)}+𝐹_{(𝑛−2)},𝐹_0=0,𝐹_1=1$

**string adalah deretan berhingga karakter berbentuk**
$a_1a_2a_3...a_n$

panjang string S adalah jumlah karakter di dalam string tersebut
     
Contoh:
1. informatika adalah string dengan panjang 11 karakter
2. 10100101 adalah string biner dengan panjang 8 bit

String kosong dilambangkan dengan $\lambda$, panjangnya = 0

### Penjumlahan Deretan

  Jumlah deretan 
	$a_m, a_{m+1}, a_{m+2}, …, a_n$
  adalah
	 $a_m + a_{m+1} + a_{m+2} + … + a_n
  atau dalam notasi sumasi:
	$\sum_{𝑘=𝑚}^𝑛𝑎_𝑘$
   
k:adalah indeks summasi
m:adalah batas bawah indeks
n:adalah batas atas indeks

Contoh 1: Berapa nilai $\sum_{𝑘=𝑚}^𝑛𝑎_𝑘$ ?
Jawaban: 
	$\sum_{(𝑘=1)}^5𝑘^2 = 12 + 22 + 32 + 42 + 52 = 1 + 4 + 9 + 16 + 25 = 55$


Contoh 2: Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda. Pada contoh 2 di atas batas bawah digeser dari 1 menjadi 0, akibatnya:
$\sum_{(𝑘=1)}^5𝑘^2= \sum_{(𝑘=0)}^4(𝑘+1)^2$

Contoh 3: Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya
$\sum_{k=1}^{100} k^2 = \sum_{k=1}^{49} k^2 + \sum_{k=50}^{100} k^2$

summation formula
| sum | closed form |
|---|---|
| $\sum_{k=0}^{n} ar^k$ ($r \neq 0$)| $\frac{ar^{n+1}-a}{r-1}$, $r \neq 1$ |
|$\sum_{k=1}^{n} k$ |$\frac{n(n+1)}{2}$ |
|$\sum_{k=1}^{n} k^2$|$\frac{n(n+1)(2n+1)}{6}$|
|$\sum_{k=1}^{n} k^3$ |$\frac{n^2(n+1)^2}{4}$|
| $\sum_{k=0}^{\infty} x^k,\|x\|<1$ | $\frac{1}{1-x}$ |
| $\sum_{k=1}^{\infty} k x^{k-1},\|x\|<1$ | $\frac{1}{(1-x)^2}$ |

### Sumasi ganda

Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.

Contoh: $\sum_{i=1}^4 \sum_{j=1}^3 i j$

Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu dilanjukan dengan sumasi terluar:
$$
\sum_{i=1}^4 \sum_{j=1}^3 i j=\sum_{i=1}^4(i+2 i+3 i)=\sum_{i=1}^4 6 i=6+12+18+24=60
$$

## Rekursif

### Pengertian

Sebuah objek dikatakan rekursif  (recursive) jika ia didefinisikan dalam terminologi dirinya sendiri. 

Proses mendefinisikan objek dalam terminologi dirinya sendiri disebut rekursi (recursion).

### Fungsi Rekursif

Fungsi rekursif didefinisikan oleh dua bagian:
#### 1. Basis 
* Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit. 
* Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
 
#### 2. Rekurens
* Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri. 
* Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil. 

Contoh : Misalkan $f$ didefinsikan secara rekusif sbb
$$
f(n)=\left\{\begin{array}{cll}
3 & , n=0 & \text { basis } \\
2 f(n-1)+4 & , n>0 & \text { rekurens }
\end{array}\right.
$$

Tentukan nilai $\mathrm{f}(4)$ !
$$
\text { Solusi: } \quad \begin{aligned}
& f(4)=2 f(3)+4 \\
= & 2(2 f(2)+4)+4 \\
= & 2(2(2 f(1)+4)+4)+4 \\
= & 2(2(2(2 f(0)+4)+4)+4)+4 \\
= & 2(2(2(2 \cdot 3+4)+4)+4)+4 \\
= & 2(2(2(10)+4)+4)+4 \\
= & 2(2(24)+4)+4 \\
= & 2(52)+4 \\
= & 108
\end{aligned}
$$

$$\begin{aligned}
&\text { Cara lain menghitungnya: }\\
&\begin{aligned}
& \mathrm{f}(0)=3 \\
& \mathrm{f}(1)=2 \mathrm{f}(0)+4=2 \cdot 3+4=10 \\
& \mathrm{f}(2)=2 \mathrm{f}(1)+4=2 \cdot 10+4=24 \\
& \mathrm{f}(3)=2 \mathrm{f}(2)+4=2 \cdot 24+4=52 \\
& \mathrm{f}(4)=2 \mathrm{f}(3)+4=2 \cdot 52+4=108
\end{aligned}\\
&\text { Jadi, } f(4)=108
\end{aligned}$$

### Latihan

1. Definisikan an secara rekursif , yang dalam hal ini a adalah bilangan riil tidak-nol dan n adalah bilangan bulat tidak-negatif.

2. Nyatakan a x b secara rekursif, yang dalam hal ini a dan b adalah bilangan bulat positif.

Solusi : 

$1 \cdot a^n=\underbrace{a \cdot a \cdot a \cdot \ldots a}_{n \mathrm{kali}}=a \cdot \underbrace{a \cdot a \cdot a \cdot \ldots a}_{n-1 \mathrm{kali}}=a \cdot a^{n-1}$
sehingga:
$$
a^n=\left\{\begin{array}{cc}
1 & , n=0 \\
a \cdot a^{n-1} & , n>0
\end{array}\right.
$$
2.
$$
\begin{aligned}
a \cdot b & =\underbrace{b+b+b+\ldots+b}_{a \text { kali }} \\
& =b+\underbrace{b+b+\ldots+b}_{a-1 \mathrm{kali}} \\
& =b+(a-1) b
\end{aligned} \longrightarrow a \cdot b=\left\{\begin{array}{cc}
b & , a=1 \\
b+(a-1) b & , a>1
\end{array}\right. \text {. }
$$