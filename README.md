```
# Cara Menambah Repository ke Software Update OpenWrt

## Langkah-langkah Instalasi dan Konfigurasi

1. **Akses IP LuCI Router Anda:**
   - Buka browser dan masukkan alamat IP router Anda, contohnya: `192.168.1.1`.

2. **Login ke LuCI:**
   - Masukkan kredensial login Anda untuk mengakses antarmuka LuCI.

3. **Navigasi ke Konfigurasi Software:**
   - Setelah login, buka tab "System" -> "Software" -> "Configuration".

### Mengubah Konfigurasi

Tambahkan tanda `#` (pagar) di depan baris `option check_signature`. Berikut adalah contoh perubahan:

Dari:

```
option check_signature
```

Menjadi:

```
# option check_signature
```

### Menambahkan Custom Feeds

Tambahkan custom feeds ke bagian "Custom Feeds". Contoh:

```
src/gz custom_arch https://raw.githubusercontent.com/fyn170/my-package/main/aarch64_cortex-a53
```


---
