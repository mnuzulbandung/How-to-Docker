### How to: Menge-Push Docker Image ke Docker Hub

1.	Buka Docker Desktop; lalu login.

2.	Buka command prompt; lalu login akun docker dengan menjalankan script berikut.

```
    docker login
```

3.	Dalam command prompt, buka daftar Docker Images yang dimiliki dengan menjalankan script berikut.

```
    docker images
```

4.	Pada daftar Docker Images Poin 2, copy nama Docker Image yang ingin di-push (Contoh, docker_sample_mnuzulbandung01: v.0.01)

5.	Dalam command prompt, lakukan tag dengan nama repository pada Docker Hub dengan menjalankan script berikut. docker_sample_mnuzulbandung01: v.0.01 merupakan nama dari Docker Image yang ingin di-push. mnuzul973 merupakan nama username akun Docker.

```
    docker tag docker_sample_mnuzulbandung01:v.0.01 mnuzul973/docker_sample_mnuzulbandung01:v.0.01
```

6.	Dalam command prompt, lakukan push Docker Image ke Docker Hub dengan menjalankan script berikut. 52db50f60b5b merupakan ID dari Docker Image yang ingin di-push. mnuzul973 merupakan nama username akun Docker.

```
    docker push mnuzul973/docker_sample_mnuzulbandung01:v.0.01
```

7.	Pastikan Docker Image ada pada Docker Hub dengan buka laman Docker Hub; login dengan akun Docker; dan cek repositori. 
