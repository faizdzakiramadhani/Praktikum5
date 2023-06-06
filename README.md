# Basis-data-praktikum-5

```
Latihan
1 Lakukan join table Mahasiswa dan Dosen
2 Lakukan join tabel Matakuliah dan Dosen
3 Lakukan join table JadwalMengajar, Dosen, dan Matakuluan
4 Lakukan join tabel KrsMahasiswa, Mahasiswa, Matakuliah, dan Dosen
```
### Tabel Mahasiswa
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/d87072dd-dcec-4798-9aa8-0ba89d4ae027)

![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/318eb4e6-15f6-490d-aae8-f121a05e548b)

### Tabel KrsMahasiswa
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/a5ee6dab-3ec3-42c0-a9e0-d063446b9d38)

### Tabel JadwalMengajar
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/0a656dd3-09c8-41fe-8a2b-ddc5b0fd23d6)

### Tabel Matakuliah
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/e4575727-ae39-4ec6-a550-e7eb3931bd6e)

# LATIHAN

1 Lakukan join table Mahasiswa dan Dosen
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/46d51433-a6ee-4fb5-95a5-90357a6af0d0)

2 Lakukan join tabel Matakuliah dan Dosen
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/8ea5fffc-cdfa-41aa-8a4f-3b99acacee5f)

```
Pada kode ini hasilnya tabel dosen null karena kedua tabel tidak saling ber relasi
```


3 Lakukan join table JadwalMengajar, Dosen, dan Matakuluan
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/d0e2ed3a-f728-40ac-b6f6-db8061f572c9)

4 Lakukan join tabel KrsMahasiswa, Mahasiswa, Matakuliah, dan Dosen
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/6f956aba-0dcb-4cbb-8e73-596001f4deb5)

# LATIHAN

1. JOIN table Mahasiswa dan Dosen
```
SELECT Mahasiswa.nim, Mahasiswa.nama, Mahasiswa.jenis_kelamin, Dosen.nama AS 'Dosen' 
FROM Mahasiswa 
JOIN Dosen ON Dosen.kd_ds=Mahasiswa.kd_ds;
```
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/51c8e426-9e38-48e7-8dc3-d7a13cdf9a68)


2. LEFT JOIN table Mahasiswa dan Dosen
```
SELECT Mahasiswa.nim, Mahasiswa.nama, Mahasiswa.jenis_kelamin, Dosen.nama AS 'Dosen'
FROM Mahasiswa
LEFT JOIN Dosen ON Dosen.kd_ds=Mahasiswa.kd_ds;
```
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/cf7db06e-ffc1-4e07-a516-e4e29bc7f361)


3. JOIN table JadwalMengajar, Dosen, dan Matakuliah
```
SELECT jadwalMengajar.kd_mk, matakuliah.nama AS 'Mata kuliah', matakuliah.sks, Dosen.nama AS 'Dosen Pengampu'
FROM jadwalMengajar
JOIN Dosen ON jadwalMengajar.kd_ds = Dosen.kd_ds
JOIN matakuliah ON jadwalMengajar.kd_mk = matakuliah.kd_mk;
```
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/f54453ca-72c3-4834-b0b1-d443ec85900b)

4. JOIN table JadwalMengajar, Dosen, dan Matakuliah
```
SELECT jadwalMengajar.kd_mk, matakuliah.nama AS 'Mata kuliah', matakuliah.sks, Dosen.nama AS 'Dosen Pengampu', jadwalMengajar.hari, jadwalMengajar.jam, jadwalMengajar.ruang
FROM jadwalMengajar
JOIN Dosen ON jadwalMengajar.kd_ds = Dosen.kd_ds
JOIN matakuliah ON jadwalMengajar.kd_mk = matakuliah.kd_mk;
```
![image](https://github.com/faizdzakiramadhani/Praktikum5/assets/115913915/5cb9503f-9671-48d4-a45a-6c41fc91f33c)
















