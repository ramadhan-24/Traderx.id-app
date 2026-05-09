SETUP TRADER X ACADEMY - GOOGLE LOGIN + FIRESTORE

1. Buka https://console.firebase.google.com/
2. Create Project: Trader X Academy
3. Masuk Build > Authentication > Get started
4. Masuk Sign-in method > aktifkan Google
5. Masuk Build > Firestore Database > Create database
6. Pilih region database, lalu buat database
7. Masuk Firestore Database > Rules
8. Copy isi file firestore_rules_traderx.rules ke Rules, lalu Publish
9. Masuk Project Settings > General > Your apps > pilih Web app
10. Copy firebaseConfig
11. Buka file traderx_academy_google_firestore.html
12. Cari bagian:

const firebaseConfig = {
  apiKey: "ISI_API_KEY_FIREBASE_LU",
  authDomain: "ISI_AUTH_DOMAIN_FIREBASE_LU",
  projectId: "ISI_PROJECT_ID_FIREBASE_LU",
  storageBucket: "ISI_STORAGE_BUCKET_FIREBASE_LU",
  messagingSenderId: "ISI_MESSAGING_SENDER_ID_FIREBASE_LU",
  appId: "ISI_APP_ID_FIREBASE_LU"
};

13. Ganti dengan config dari Firebase.
14. Jalankan pakai Live Server / localhost / Firebase Hosting.

CATATAN:
- Jangan langsung buka dari file:// kalau Google Login gagal.
- Di Firebase Authentication > Settings > Authorized domains, pastikan domain kamu ada.
- Untuk uji lokal biasanya localhost sudah aman.
- Data user tersimpan di:
  users/{uid}/profile/main
  users/{uid}/journal/{tradeId}
