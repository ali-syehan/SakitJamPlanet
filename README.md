# Ali Syehan WebView APK

Project ini mengubah file HTML/JS menjadi aplikasi Android WebView.

## Struktur penting

- `app/src/main/assets/index.html` = halaman utama aplikasi.
- `app/src/main/assets/js/allRowsData.js` = database JavaScript yang dibaca oleh `index.html`.
- `.github/workflows/build-webview-apk.yml` = workflow GitHub Actions untuk membuat APK.

## Nama workflow

**Build WebView APK**

## Cara pakai di GitHub

1. Buat repository baru di GitHub.
2. Upload semua isi folder project ini ke repository tersebut.
3. Masuk tab **Actions**.
4. Pilih workflow **Build WebView APK**.
5. Klik **Run workflow** atau push ke branch `main`.
6. Setelah selesai, buka hasil run workflow.
7. Download artifact bernama **AliSyehan-WebView-debug-apk**.
8. Di dalam artifact tersebut ada file `app-debug.apk`.

## Update data

Untuk mengganti database, cukup ganti file:

`app/src/main/assets/js/allRowsData.js`

Pastikan nama variabel tetap:

```js
const allRowsData = [
  // data...
];
```
