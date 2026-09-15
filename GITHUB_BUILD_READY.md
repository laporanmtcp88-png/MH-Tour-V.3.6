# MH Tour — GitHub Build Ready

Paket ini sudah disusun dengan struktur yang dapat langsung di-upload ke repository GitHub.

## Struktur root

- `.github/workflows/build-release-signed.yml`
- `android/`
- `server/`
- `tools/`
- `.gitignore`
- `README.md`

## GitHub Actions

Workflow menggunakan:
- JDK 17
- Gradle 8.11.1
- Android SDK 35
- Debug APK
- Release APK dengan temporary CI signing key

Tidak membutuhkan GitHub Secrets untuk build pengujian pertama.

Setelah build berhasil, artifact bernama `MH-Tour-APK` berisi:
- `MH_Tour_Debug.apk`
- `MH_Tour_Release_CI_Signed.apk`

**Catatan:** Release CI signed menggunakan kunci sementara. Untuk APK produksi yang akan menerima update aplikasi di masa depan, gunakan keystore produksi yang tetap.
