
### **🔄 Alur Kerja Kolaborasi**  
Setiap anggota bekerja di branch-nya sendiri.  
Contoh: Yudha bekerja di branch `yudha`.  

**Setelah selesai bekerja harian, push ke branch masing-masing:**  
```bash
git add .
git commit -m "Deskripsi singkat update"
git push origin fitur-nama
```

---

## **👨‍💻 PANDUAN UNTUK SEMUA ANGGOTA TIM**  

### **✅ 1. Clone Project dari GitHub** *(Hanya dilakukan sekali)*  
```bash
git clone https://github.com/mbok-rondo/mbok-rondo-game.git
cd mbok-rondo-game
```

### **🔁 2. Ambil Update Terbaru dari `master`** *(Lakukan setiap hari)*  
```bash
git checkout master
git pull origin master
```

### **🌿 3. Pindah ke Branch Pribadi**  
```bash
git checkout nama-kamu
# Contoh: git checkout yudha
```

### **🎨 4. Kerjakan Fitur Kamu**  
Lakukan perubahan di Unity seperti biasa.  

### **⬆️ 5. Simpan dan Push Pekerjaan ke Branch Sendiri** *(Setelah selesai harian/milestone kecil)*  
```bash
git add .
git commit -m "Deskripsi perubahan, contoh: Tambah animasi NPC wanita"
git push origin fitur-nama-kamu
# Contoh: git push origin yudha
```

### **🔄 6. Setelah Admin Merge, Ambil Update Terbaru Lagi dari `master`**  
```bash
git checkout master
git pull origin master
git checkout nama-kamu
git merge master
```

---

## **🧑‍💼 PANDUAN UNTUK ADMIN (NABIL)**  

### **✅ 1. Ambil Semua Update dari Semua Branch**  
```bash
git fetch --all
```

### **🔍 2. Cek dan Uji Setiap Branch Sebelum Merge**  

### **🔄 3. Merge ke Branch `master`**  
```bash
git checkout master
git pull origin master  # Pastikan master versi terbaru
git merge yazid
git merge hilmy
git merge yudha
git merge echo
git merge nabil
```

### **⬆️ 4. Push ke Remote `master`**  
```bash
git push origin master
```

### **📣 5. Beritahu Semua Anggota untuk Update Project**  
Anggota tinggal menjalankan:  
```bash
git checkout master
git pull origin master
git checkout fitur-nama
git merge master
```

--- 

Dengan struktur ini, panduan lebih mudah dibaca dan diikuti oleh seluruh anggota tim.
