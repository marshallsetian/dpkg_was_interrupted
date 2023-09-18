# dpkg_was_interrupted
manually run sudo dpkg configure a to correct the problem (linux0S)

bisa di pakai saat kamu ada problem seperti kasus saya di kali linux 0S

problem tersebut di terangkan via terminal ketika menjalankan perintah 
# sudo apt upgrade 
++++
dpkg was interrupted, you must manually run sudo dpkg –configure -a to correct the problem

jika kalian menemukan masalah seperti ini bisa kalian coba dengan mengetikkan perintah di terminal :
opsi membuka terminal bisa di lakukan dengan menekan tombol
"CTRL + ALT + T",

ketikkan :

sudo rm /var/lib/apt/lists/lock
katikkan lagi :
sudo rm /var/cache/apt/archives/lock
ketikkan lagi :
cd /var/lib/dpkg/updates
ketikkan lagi :
sudo rm *
ketikkan lagi :
sudo apt-get update

jika setelah upgrade atau ingin memasang / install aplikasi tetapi masih menghasilkan pesan yang sama "dpkg was interrupted, you must manually run sudo dpkg –configure -a to correct the problem", 
coba dengan perintah lainnya dibawah ini akan tetapi kalian harus terhubung dengan internet,
berikut adalah perintahnya :

sudo dpkg --configure -a
ketikkan lagi :
sudo apt-get install -f

semoga bisa membantu masalah teman2 sekalian mengatasi problem upgrade error disini...
