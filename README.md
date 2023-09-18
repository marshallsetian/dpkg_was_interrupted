<h1><p align="center">MENGATASI MASALAH UPGRADE - UPDATE VIA TERMINAL LINUX OS</p>
<p align="center">
<h1>
</p>
<p align="center">
<a href="#"><img title="BRUTAL SPAM WHATSAPP" src="https://img.shields.io/badge/mengatasi masalah upgrade linux os-green?colorA=%23ff0000&colorB=%23017e40&style=for-the-badge"></a>
</p>
<p align="center">
manually run sudo dpkg configure a to correct the problem (linux0S)<h1></h1>


bisa di pakai saat kamu ada problem seperti kasus saya di kali linux 0S

problem tersebut di terangkan via terminal ketika menjalankan perintah :</p>
## sudo apt upgrade</p>
 output keluaran :

### dpkg was interrupted, you must manually run sudo dpkg –configure -a to correct the problem
</p>

jika kalian menemukan masalah seperti ini bisa kalian coba dengan mengetikkan perintah di terminal :
opsi membuka terminal bisa di lakukan dengan menekan tombol
"CTRL + ALT + T",

ketikkan :
```bash
sudo rm /var/lib/apt/lists/lock
```
ketikkan lagi :
```bash
sudo rm /var/cache/apt/archives/lock
```
ketikkan lagi :
```bash
cd /var/lib/dpkg/updates
```
ketikkan lagi :
```bash
sudo rm *
```
ketikkan lagi :
```bash
sudo apt-get update
```
</p>

jika setelah upgrade atau ingin memasang / install aplikasi tetapi masih menghasilkan pesan yang sama 
### "dpkg was interrupted, you must manually run sudo dpkg –configure -a to correct the problem"

coba dengan perintah lainnya dibawah ini akan tetapi kalian harus terhubung dengan internet,
berikut adalah perintahnya :
```bash
sudo dpkg --configure -a
```
ketikkan lagi :
```bash
sudo apt-get install -f
```

semoga bisa membantu masalah teman2 sekalian mengatasi problem upgrade error disini...
