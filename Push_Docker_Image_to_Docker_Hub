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

4.	Pada daftar Docker Images Poin 2, copy IMAGE ID dari Docker Image yang ingin di-push (Contoh, 52db50f60b5b)

5.	Dalam command prompt, lakukan tag dengan nama repository pada Docker Hub dengan menjalankan script berikut. 52db50f60b5b merupakan ID dari Docker Image yang ingin di-push. mnuzul973 merupakan nama username akun Docker. docker_sample merupakan nama repository target push Docker Image.

```
    docker tag 52db50f60b5b mnuzul973/docker_sample
```

6.	Dalam command prompt, lakukan push Docker Image ke Docker Hub dengan menjalankan script berikut. 52db50f60b5b merupakan ID dari Docker Image yang ingin di-push. mnuzul973 merupakan nama username akun Docker. docker_sample merupakan nama repository target push Docker Image.

```
    docker push 52db50f60b5b mnuzul973/docker_sample
```

7.	Pastikan Docker Image ada pada Docker Hub dengan buka laman Docker Hub; login dengan akun Docker; dan cek repositori. 
