# Sys Engine Job Desc
## Bios Setting
1. BIOS version : 311 
2. GPU information : Intel(R) UHD Graphics, NVIDIA GeForce RTX 3050
3. CPU : 11th Gen Intel(R) core(™) i5-11400H @ 2.70G
4. Storage : PCIE Bud:2 Dev:0 Func:0
5. Device Type: NVMe SSD (512.1GB)
6. Model Name: WD PC SN735


### Layout Hardisk
**[Tabel Hardisk]** ](https://drive.google.com/file/d/18g-i7H5FQtV4mfxozLl0Wd8M5H2fF0HF/view?usp=drive_link)

1. cryptsetup luksFormat /dev/nvme0n1p6 
2. cryptsetup luksOpen /dev/nvme0n1p6 geps 
3. pvcreate /dev/mapper/geps 
4. Vgcreate vol /dev/mapper/geps 
5. lvcreate –l100%FREE –n root vol 

### Yang perlu di install
1. Linux-hardened 
2. Linux-zen 
3. Linux-firmware 
4. Intel-ucode 
5. Base base-devel 
6. Mkinitcpio 
7. Neovim 
8. Lvm2 
9. Vim 
10. Git 
11. Iwd

### Configurasi yang di lakukan
1. Konfigurasi network protocol time 
2. Konfigurasi locale 
3. Konfigurasi hostname dan host 
4. Konfigurasi user administrasi 
5. Konfigurasi boot 
6. Konfigurasi inagw linux custom

### Yang perlu di install saat installing tampilan 
1. Hyprland 
2. Polkit polkit-gnome 
3. Pipewire pipewire-pulse 
4. Nerd-fonts 
5. Wireplumber 
6. Swaync 
7. Nautilus 
8. Kitty 
9. Wofi 
10. Waybar


# Deployer Job Desc
## Install Aplikasi Media Wiki
1. install docker
2. install docker-compose
3. git clone database dari github
4. buat file lym
5. pulling file mediawiki ke file mediawiki-docker
6. running media wiki dengan docker compose
7. docker compose start
8. buka aplikasi media wiki di browser dengan port 80 (localhost:80)


# Network Engine Job Desc

1. pacman -S firewalld :
untuk menginstall firewall

2. firewall-cmd --list-all-zones :
untuk melihat list semua zone yang sudah ada

3. firewall-cmd --dmz --remove-service ssh :
untuk mengganti zone yang ingin di ganti

4. firewall-cmd --zone=public --add-service http :
untuk menambah zone yang ingin ditambah

5. firewall-cmd --zone=public --add-port=80/tcp :
untuk menambah port yang di perlukan

6. firewall-cmd --reload :
untuk memuat ulang perubahan yang sudah di ganti


# Contentn Research Job Desc
1. Berikan kata sambutan dan pengenalan untuk mengisi pembukaan dari web wiki ini
2. Memilih apa saja konten yang ada didalamnya, terkait dengan perpustakaan
3. Menyaring konten yang sekiranya paling banyak dicari oleh para pengguna
4. Setelah mendapat kontennya, masukkan itu sebagai hyperlink yang nantinya akan berisi konten yang dicari
5. Selanjutnya isi hyperlink itu dengan link website yang sudah dipilih dari website terpercaya
6. Setelah semua konten yang sekiranya menjadi top penelusuran sudah dimasukkan, simpan progersnnya
7. Terakhir, merapihkan bagian bagian yang dirasa kurang atau lebih terkait isi konten tersebut


