### How to: Membuat Docker Images dan memasukkannya ke dalam Docker Desktop

1. Buat folder dengan nama apa pun di lokasi mana saja.

2. Masukan aplikasi yang ingin dikemas (Contoh, app.py) ke dalam folder poin 1. Berikut contoh dari aplikasi yang ingin dikemas.

   ```
    import pandas as pd

    def data():
    data = {'Name': ['Adi', 'Budi', 'Cindi', 'Dedi'],
    'Age': [15, 16, 17, 18]}
    df = pd.DataFrame(data)
    print(df)

    if __name__== '__main__':
        data()
   ```

3.	Masukkan file requirement.txt ke dalam folder Poin 1. File ini berisi library beserta versinya yang diperlukan untuk menjalankan aplikasi yang ingin dikemas. Lihat link ini untuk cara membuatnya.

4.	Cari tahu versi python yang digunakan untuk menjalankan aplikasi yang ingin dikemas. Lihat link ini untuk cara melihatnya.

5.	Buat docker file bernama 'Dockerfile' (tanpa ada extensi dengan huruf kapital di depan). Masukkan Dockerfile ke dalam folder yang dibuat pada Poin 1. Berikut contoh dari Dockerfile. Pastikan versi python sesuai dengan Poin 4.

```
    FROM python:3.9.20
    COPY . /
    RUN pip install -r requirements.txt
    CMD ["python", "app.py"]
```

6.	Buka Docker Desktop; lalu login.

7.	Buka command prompt; lalu login akun docker dengan menjalankan script berikut.

```
    docker login
```

8.	Buka command prompt; pergi ke folder Poin 1; lalu buat Docker Images dengan menjalankan script berikut. docker_sample_mnuzulbandung01 merupakan nama dari Docker Images yang akan dibuat. v.0.01 merupakan versi dari aplikasi tersebut.

```
    docker build -t docker_sample_mnuzulbandung01:v.0.01 .
```

9.	Jika poin 8 berhasil, di dalam Docker Desktop, di bagian Images, akan terdapat Docker Images bernama docker_sample_mnuzulbandung01. Hal ini juga bisa dilakukan dengan menjalankan script berikut di dalam command promt.

```
    docker images
```
