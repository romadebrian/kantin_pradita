# aplikasi kantin Pradita
Aplikasi kantin sederhana dengan php dan mysql

Fitur
- Login
- Pesan makanan
- Menambah daftar makanan
- Membuat laporan hasil bulanan
- Bisa di cetak

Yang harus di kerjakan
- Membuat tampilan memesan makanan untuk pelanggan yang nantinya di jadikan struk (menu utama setelah login dan berbasis GUI/Gambar/Table)
- Membuat logs login untuk kemanan (id, IP, MAC Address)

Alur Program pemesanan
- Pilih warung
- Pilih makanan
- Print sruk
- Pilih warung yang lain
- Pilih makan
- Print struk untuk warung itu aja

Konsep
Cust ingin makan warteg yg dikantin, nah cust harus ke kasir dulu, kasir inputin makan yg di inginkan cust, nah warteg ini nih harus buat fix menu yg ga berubah2 (karna kan kita tau warteg kantin ini menunya gonta ganti kan) , setelah kasir input menu yg di pengen cust, kasir ngasih struk nya ke cust, cust bawa struk buat dikasih ke tenant warteg, warteg buatin pesenan nya dsn nyimpen struk itu yang mana struknya pas closing operation harus di tukerin ke kasir buat dpt uang, nanti kasir pas closing operation input total struk masing2 tenant, misalkan tenant warteg 10struk, baso 5struk, dsb nya.

Question & answer :
Gimana kalo cust mesen makanan 2 tenant ? Semisal cust mesen geprek di tenant kuning, trus mesen baso di tenant baso
Jawaban nya gabisa, jadi kasir harus input 2 kali, buat ngehasil 2 struk yg bakalan dikasih ke cust

Question & answer 2 :
Gimana kalo cust ngilangin struknya sblm di tukerin jd makanan ? Ya cust gabakal bisa dpt makanan, meskipun si cust udh bayar.
Kenapa ga dpt makanan? Ya karna tenant bakalan bisa dpt uang kalo ada struk
Jd apabila tenant ngeluarin makanan tanpa struk, trus si tenant minta uang ke kasir. Ya gabisa
Jadi tenant maupun cust kudu jaga baik2 dah tuh struk
Fungsi struk buat tenant itu buat nukerin jd uang, pas close order bakal di itung sm kasir jumlah struknya brp

Question & answer 3 :
Gimana kalo tenant pengen nukerin struk jd uang sblm close operation?
Struk gabisa di tukerin sblm close operation, jadi tenant harus nunggu sampe close operation jam 5 sore buat di itung report harian per tenant.
Kalo tenant nukerin struk jam 3, otomatis sistem kasir nya juga close, yg berarti gabisa ada yg order lg kalo udh 
