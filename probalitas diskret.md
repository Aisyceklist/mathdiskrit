---
title: probalitas diskret

---

# PROBALITAS
Probabilitas adalah cabang dari matematika yang mempelajari tentang kemungkinan terjadinya suatu peristiwa. Sederhananya, probabilitas adalah ukuran seberapa sering suatu kejadian diharapkan terjadi.
## PROBALITAS DISKRIT
### pengertian
Probabilitas diskret adalah peluang yang berhubungan dengan variabel acak diskret, yaitu variabel yang hanya dapat mengambil nilai tertentu (terhitung). Contoh: hasil lemparan dadu ({1, 2, 3, 4, 5, 6}) atau lemparan koin ({Head, Tail}).

* Ruang Sampel (S): Semua kemungkinan hasil dari suatu percobaan.
Contoh: Melempar koin sekali, $S = \{Head, Tail\}$
* Peristiwa (A): Subset dari ruang sampel.
Contoh: Mendapatkan Head,$A = \{Head\}$
* Probalitas Peristiwa: $P(A) = \frac{\text{Jumlah elemen A}}{\text{Jumlah elemen S}}$
* Melempar dadu, probabilitas mendapatkan angka genap ({2, 4, 6}): $P(\text{genap}) = \frac{3}{6} = 0.5$
## PROBALITAS BAYESIAN
### pengertian
Probabilitas Bayesian adalah pendekatan probabilitas yang menggunakan informasi awal (prior) untuk memperbarui peluang ketika informasi baru (evidence) muncul. PTeorema Bayes membantu kita menghitung probabilitas suatu hipotesis (H) diberikan bukti (E).

Rumusnya: $P(H|E) = [P(E|H) * P(H)] / P(E)$

$P(H|E)$: Probabilitas hipotesis (H) benar, diberikan bukti (E).
$P(E|H)$: Probabilitas memperoleh bukti (E), jika hipotesis (H) benar.
$P(H)$: Probabilitas hipotesis (H) benar sebelum melihat bukti.
$P(E)$: Probabilitas mendapatkan bukti (E) tanpa memandang hipotesis.