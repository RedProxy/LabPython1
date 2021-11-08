# LabPython1

## Lab 2: Struktur Kondisi
### Latihan 1
#### Program dan Output
#### Program sederhana dengan input 2 buah bilangan serta menentukan bilangan terbesar dari kedua bilangan
- Program Menentukan Bilangan Terbesar dari 2 Buah Bilangan

    ```bash
    print("Program Menentukan Bilangan Terbesar")
    print("====================================")

    a = int(input("Masukan nilai a: "))
    b = int(input("Masukan nilai b: "))

    if a > b:
        maks = a
    else:
        maks = b
    print('Nilai Terbesar adalah %d' % maks)
    ```
    ![IMG 1](screenshoot/Lab2Lat1.1.png)

- Output

    ![IMG 2](screenshoot/Lab2Lat1.2.png)

### Latihan 2
#### Program dan Output
#### Program mengurutkan data berdasarkan input jumlah data serta menentukan urutan dari data terkecil
- Program mengurutkan data berdasarkan input jumlah data serta menentukan urutan dari data terkecil

     ```bash
    print('Program mengurutkan data')
    angka = []
    def mengurut(angka):
        a = int(input("Bilangan ke-1:"))
        angka.append(a)
        b = int(input("Bilangan ke-2:"))
        angka.append(b)
        c = int(input("Bilangan ke-3:"))
        angka.append(c)
        tukar = True
        while tukar:
            tukar=False
            for n in range(len(angka)-1):
                if angka[n] > angka[n+1]:
                    angka[n], angka[n+1] = angka[n+1], angka[n]
                    tukar = True
        return angka
    print("Urutan Bilangan:",mengurut(angka))
    ```
    ![IMG 3](screenshoot/Lab2Lat2.1.png)

- Output

    ![IMG 4](screenshoot/Lab2Lat2.2.png)

## Lab 3: Perulangan
### Latihan 1
#### Program dan Output
#### Program Perulangan Bertingkat
- Program

    ```bash
    #Program Perulangan

    for i in range(0, 10):
        for j in range(10):
            print('%3d'%(i+j), end = ' ')
        print(' ')
    ```

    ![IMG 5](screenshoot/Lab3Lat1.1.png)

- Output

    ![IMG 6](screenshoot/Lab3Lat1.2.png)

### Latihan 2
#### Program dan Output
- Tampilkan n bilangan acak yang lebih kecil dari 0.5
- Nilai n diisi pada saat runtime
- Anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya

- Program 

    ```bash
    from random import random
    n = int(input("Masukan Nilai N: "))
    for i in range(n):
        while 1:
            n = random()
            if n < 0.5:
                break
        print(n)
    ```
   ![IMG 7](screenshoot/Lab3Lat2.1.png) 

- Output

    ![IMG 8](screenshoot/Lab3Lat2.2.png) 

# TERIMA KASIH