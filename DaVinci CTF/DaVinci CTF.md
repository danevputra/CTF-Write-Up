# Authentication 

Kita diminta untuk login sebagai admin, 
Langsung saja menggunakan sql injection
Username : admin
Password : ‘or’’=’

Flag : dvCTF{!th4t_w4s_34sy!}

# Read

Kita diminta untuk memperbaiki gambar yang sudah dirusak dengan gaussian noise

Kita menggunakan tools stegsolve, dengan stereogram solver dengan offset 160, dan didapatkan hasil sebagai berikut :


Flag : dvCTF{th4t5_4_l0t_0f_n0153}

# Pidieff
Diberikan sebuah PDF setelah dilakukan pengecekan menggunakan strings ternyata ditemukan ada file flag.txt

Setelah itu kami menggunakan perintah  
pdf-parser --stats super_secret.pdf  dan hasilnya



Ada embeddedfile dengan id 3 selanjutnya dilakukan extract data
pdf-parser --object 3 --raw --filter super_secret.pdf > text

Flag : dvCTF{look_at_the_files}


# Substitution
Diberikan sebuah cipher, sesuai namanya kami langsung menembak 

Flag : dvCTF{cr1pt3d_c1ph3r}
