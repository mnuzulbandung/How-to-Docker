### How to: Menjalankan Docker Images dan membuat Docker Container

1.	Buka command prompt; lalu login akun docker dengan menjalankan script berikut.

```
    docker login
```

2. Dalam command prompt, jalankan script berikut. docker_sample_mnuzulbandung01:v.0.01 merupakan nama Docker Image yang ingin dijalankan. container_mnuzulbandung01 merupakan nama Docker Container yang ingin dibuat.

```
    docker run -t --name container_mnuzulbandung01 docker_sample_mnuzulbandung01:v.0.01
```

3.	Poin 2 juga bisa dilakukan dengan Docker Desktop. Buka Docker Desktop; masuk ke bagian images; pilih Docker Images yang ingin dijalankan; klik bagian yang ditandai kotak merah.

4. Isi informasi dari nama container yang ingin dibuat beserta nomor portnya.
