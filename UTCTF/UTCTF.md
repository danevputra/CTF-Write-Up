# Sanity Check
Hanya join server discord dan di announcement sudah ada flagnya
Flag : utflag{welcome_to_utctf}
HTML
Diberikan sebuah website, dan setelah dicoba membuka source code maka flag ditemukan

Flag : utflag{you_found_me_0123959}

# Stringy Things 
Diberikan sebuah files, dan sesuai namanya kami mencoba untuk melakukan strings pada file tersebut 

Flag : utflag{strings_is_op}

# Magic Bytes
Diberikan sebuah file out.txt. Setelah dilakukan strings tenyata kami mendapati bahwa file tersebut dibuat dengan GIMPW dimana itu indentik dengan gambar 

Setelah itu kami merubah extensi nya menjadi PNG dan mendapatkan Flag

Flag: utflag{file_extensions_mean_nothing}

# Run-ELF
Diberikan sebuah file bernama run, lalu kami mencoba menjalankannya

Flag : utflag{run_run_binary_9312854}

# Chiper Gauntlet
Diberikan banyak bilangan biner, setelah diconvert menghasilkan :
Uh-oh, looks like we have another block of text, with some sort of special encoding. Can you figure out what this encoding is? (hint: if you look carefully, you'll notice that there only characters present are A-Z, a-z, 0-9, and sometimes / and +. See if you can find an encoding that looks like this one.)
TmV3IGNoYWxsZW5nZSEgQ2FuIHlvdSBmaWd1cmUgb3V0IHdoYXQncyBnb2luZyBvbiBoZXJlPyBJdCBsb29rcyBsaWtlIHRoZSBsZXR0ZXJzIGFyZSBzaGlmdGVkIGJ5IHNvbWUgY29uc3RhbnQuIChoaW50OiB5b3UgbWlnaHQgd2FudCB0byBzdGFydCBsb29raW5nIHVwIFJvbWFuIHBlb3BsZSkuCm15eHFia2Rldmtkc3l4YyEgaXllIHJrZm8gcHN4c2Nyb24gZHJvIGxvcXN4eG9iIG1iaXpkeXFia3pyaSBtcmt2dm94cW8uIHJvYm8gc2MgayBwdmtxIHB5YiBrdnYgaXllYiBya2JuIG9wcHliZGM6IGVkcHZrcXt4eWdfaXllYm9fenZraXN4cV9nc2RyX21iaXpkeX0uIGl5ZSBnc3Z2IHBzeG4gZHJrZCBrIHZ5ZCB5cCBtYml6ZHlxYmt6cmkgc2MgbGVzdm5zeHEgeXBwIGRyc2MgY3liZCB5cCBsa2NzbSB1eHlndm9ucW8sIGt4biBzZCBib2t2dmkgc2MgeHlkIGN5IGxrbiBrcGRvYiBrdnYuIHJ5em8gaXllIG94dHlpb24gZHJvIG1ya3Z2b3hxbyE=

Bagian yang ternkripsi kami decode dengan menggunakan base64 menghasilkan 

New challenge! Can you figure out what's going on here? It looks like the letters are shifted by some constant. (hint: you might want to start looking up Roman people).
myxqbkdevkdsyxc! iye rkfo psxscron dro loqsxxob mbizdyqbkzri mrkvvoxqo. robo sc k pvkq pyb kvv iyeb rkbn oppybdc: edpvkq{xyg_iyebo_zvkisxq_gsdr_mbizdy}. iye gsvv psxn drkd k vyd yp mbizdyqbkzri sc lesvnsxq ypp drsc cybd yp lkcsm uxygvonqo, kxn sd bokvvi sc xyd cy lkn kpdob kvv. ryzo iye oxtyion dro mrkvvoxqo!

Lalu di decode lagi dengan caesar chiper dengan shift 18

Flag :utflag{now_youre_playing_with_crypto}

# Emoji Encryption
Diberikan emoji dan hanya perlu mengambil huruf depan dari setiap emoji dalam bahasa inggris
Flag : utflag{emojis_be_versatile}

# Source it
Diberikan sebuah web, setelah di cek ternyata menerapkan keamanan 
function checkPassword(form) { 
                password1 = form.password1.value; 
                name = form.name.value;
                var username = "admin";
                var hash = "1bea3a3d4bc3be1149a75b33fb8d82bc"; 
                var hashedPasswd = CryptoJS.MD5(password1);
   
                if (password1 == '') 
                    alert ("Please enter Password"); 
              
                else if (username != name) { 
                    alert ("\nYou lack access privlages...") 
                    return false; 
                }
                     
                else if (hash != hashedPasswd) { 
                    alert ("\nIncorrect password...") 
                    return false; 
                } 
  
                else{ 
                    alert("Access Granted\n" + text) 
                    return true; 
                } 
            } 

Berarti kita hanya perlu memasukkan username admin dan melakukan decode “1bea3a3d4bc3be1149a75b33fb8d82bc” md5 dimana hasilnya sherlock

Flag : utflag{b33n_th3r3_s0uRc3d_th4t}

# Shift
Diberikan sebuah gambar

Untuk mendapat flag-nya kami skew menggunakan photoshop

Setelah diperbaiki maka didapatkan :

Flag : utflag{not_when_i_shift_into_maximum_overdrive}

# Cutest Cookie Clicker Rip-Off 
Diberikan sebuah web, dengan high score 1.000.000. Kita hanya perlu mengubah cookies nya lebih tinggi dari 1 juta 

Flag : utflag{numnum_cookies_r_yumyum}

# Oinker
Diberikan sebuah web dengan input text. Nah setelah text di input, kami diarahkan ke web
http://web2.utctf.live:5320/oink/98

Kami melihat ada angka 98, dan menduga ini parameter tempering. Lalu kami menembak dan menemukan flag di http://web2.utctf.live:5320/oink/2

Flag : utflag{traversal_bad_dude} 

# Doubly Deleted Data 
Kami melakukan strings pada flash image dan mendapatkan flag 

Flag : utflag{d@t@_never_dis@ppe@rs}
