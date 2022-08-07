# Full Stack Test
### 1. Monitor area Depok pembelian bulan Juli tahun 2022 ke 12.

Digit 1-2.

- MN = Monitor
- TV = Televisi
- HD = Handfree

Digit 3 - 5 merupakan kode branch.

- DPK = Depok
- SMR = Semarang
- JK = Jogjakarta
- BL = Bali

Digit 6 - terakhir adalah bulan, tahun dan query.
- Monitor = MN
- area Depok = DPK
- bulan Juli tahun 2022 ke 12 = 07 22 12
>jawaban: MNDPK072212
---

### 2. Implementasi DRY (Don't Repeat Youtself) dalam kode berikut:
```javascript
class Worker {
  construction() {
  }
  basicSalary(){
    return this.hoursWorked * this.rate;
  }
  overviewSalary(){
    return this.hoursWorked * this.rate + this.TAX
  }
}
```

>jawaban :
```javascript
class Worker {
  construction(hoursWorked, rate, TAX) {
    this.hoursWorked = hourWorked;
    this.rate = rate;
    this.TAX = TAX;
  }
  basicSalary(){
    return this.hoursWorked * this.rate;
  }
  overviewSalary(){
    return this.basicSalary() + this.TAX
  }
}
```
---

### 3. Refactoring baris kode berikut:
```javascript
function FG() {
  let error;
  if (OK(Run1())) {
    if (OK(Run2())) {
      if (OK(Run3())) {
        if (OK(Run4())) {
        } else {
          error = Run4Err;
        }
      } else {
        error = Run3Err;
      }
      {
        error = Run2Err;
      }
    } else {
      error = Run1Err;
    }
  }
  return error;
}
```

>jawaban :

```javascript
function() {
  let error;
  
  if(!OK(RUN1)){
    error = Run1Err;
  } else if (!OK(RUN2())) {
    error = Run2Err;
  } else if (!OK(RUN3())) {
    error = Run3Err;
  } else if (!OK(RUN4())) {
    error = Run4Err;
  } else {
    return error;
  }
  
  return error;
}
```

---

### 4. CRUD pada API jsonplaceholder.typicode.com
>Link Website: https://react-trello-jsonplaceholder.vercel.app

>Link Gitub Repo: https://github.com/torik135/react-trello-jsonplaceholder
---

### 5. Munculkan semua data tiket yang open dan semua data pada rentang waktu _15 Juni 2022 - 22 Juni 2022_ berdasarkan cabang masing-masing. [PROGRESS]

- masalah database yang terlalu besar untuk di muat.
- jadi data yang dipakai hanya sekitar 700an baris data.

>solusi untuk mapping data dari database:
- solusi 1: convert baris ke kolom (groupby setelah filter dan concat).

>Link Website: in-progress.

>Link Gitub Repo: in-progress.
---

### ***Optional Challenge***.
- Input Nomor Rahasia: 1859
- Input Nomor Tebakan: 5891

Output: 1 Benar 3 Salah (8 benar, 5, 9, dan 1 salah).

>jawaban: 9815
