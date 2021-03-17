# Pollex

Kita diberikan sebuah file, kemudian kami melakukan ekstraksi dengan binwalk

Command : binwalk --dd='.*' pol

Hasil :

Sehingga didapatkan :

Flag : flag{65c34a1ec121a286600ddd48fe36bc00}

# Shoelaces
Diberikan sebuah gambar dan kami mencoba untuk mencari flag dengan string

 
Flag : flag{137288e960a3ae9b148e8a7db16a69b0}

# Read the rules
Clue : there is a flag in the source code

Flag : flag{90bc54705794a62015369fd8e86e557b}

# Esab64
Diberikan sebuah string : mxWYntnZiVjMxEjY0kDOhZWZ4cjYxIGZwQmY2ATMxEzNlFjNl13X

Kami menduga ini base64. Tetapi karena judul nya menggunakan esab atau base yang terbalik sehingga kami mengubah urutannya menjadi terbalik 

mxWYntnZiVjMxEjY0kDOhZWZ4cjYxIGZwQmY2ATMxEzNlFjNl13X

Setelah di decode menghasilkan _}e61e711106bd0db1b78efa894b1125bf{galf

Lalu kami membalik lagi urutannya agar menghasilkan flag yang benar

Flag : flag{fb5211b498afe87b1bd0db601117e16e}
