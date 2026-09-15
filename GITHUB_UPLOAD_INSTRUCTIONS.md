# Cara upload MH Tour ke GitHub

1. Ekstrak ZIP ini di komputer.
2. Upload **isi folder ini**, bukan file ZIP-nya.
3. Pastikan `.github/workflows/build-release-signed.yml` ikut ter-upload.
4. Pastikan folder `android` langsung berada di root repository.
5. Commit ke branch `main`.
6. Buka **Actions**.
7. Pilih **Build MH Tour APK**.
8. Jika belum otomatis berjalan, tekan **Run workflow** lalu pilih `main`.
9. Tunggu job **Build Android APK** sampai hijau.
10. Buka hasil run dan bagian **Artifacts**, lalu download `MH-Tour-APK`.

Jika repository sudah memiliki `.github/workflows/build-release-signed.yml` lama, file tersebut harus ditimpa dengan file dari paket ini.
