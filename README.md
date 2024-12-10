# **Docker**

Merupakan platform yang bisa dijalankan untuk mengemas suatu aplikasi dari pihak A agar bisa dijalankan oleh pihak lain secara efisien.  Selain itu, ada pula karakteristik-karakteristik lain dari Docker seperti di bawah ini:

* **Portability**. Jika suatu aplikasi sudah dikembangkan oleh pihak A, Docker dapat digunakan untuk mengemas aplikasi tersebut agar bisa dijalankan oleh pihak B (bukan pengembang) di perangkat apa saja. Pihak B tidak perlu mengkhawatirkan infrastruktur apa pun untuk menjalankan aplikasi tersebut. Pihak A dapat mengemas aplikasi menggunakan Docker ke dalam bentuk Docker Images. Lalu, Pihak B dapat membuka kembali aplikasi tersebut dengan menjalankan Docker Images ke dalam bentuk Docker Container.

* **Container Registries**. Docker Images yang dibuat oleh Pihak A dapat di-push ke container registry (seperti Docker Hub, AWS Elastic Container Registry, atau Google Container Registry) sebagai centralized storage. Lalu, Pihak B dapat menge-Pull Docker Images yang dibuat oleh Pihak A dari container registry menggunakan Docker.

* **Efficiency**. Tidak seperti Virtual Machine dimana tiap container memerlukan operating system tersendiri, Docker menggunakan kernel OS host yang bisa digunakan oleh banyak container. Kondisi ini membuat container lebih ringan dibandingkan Virtual Machine.
Isolation. Walau tiap container menggunakan kernel OS host yang sama, Docker memanfaatkan fitur seperti cgroups dan namespace di kernel Linux sehingga container berada di environment yang terisolasi. Kondisi ini membuat perubahan atau kerusakan pada satu container tidak memengaruhi container lainnya.

* **Scalability**. Karena Container bersifat ringan dan terisolasi, jika aplikasi mengalami aktivitas traffic yang tinggi, container tambahan dapat dijalankan (scaled horizontally) untuk menanganinya secara fleksibel. Lalu, container yang sedang dijalankan tidak perlu dimatikan jika ada penambahan container.


# Berikut merupakan istilah-istilah yang dipakai dalam Docker:
* **Docker Desktop**: Aplikasi Docker yang dijalankan di Local dan digunakan untuk mengemas dan membuka aplikasi (Docker Images).
* **Dockerfile**: File yang dibutuhkan untuk mengemas aplikasi.
* **Docker Images**: Bentuk aplikasi yang sudah dikemas menggunakan Docker oleh Pihak A.
* **Docker Container**: Bentuk aplikasi yang sudah dibuka dari Docker Images dan dapat dijalankan oleh Pihak B.
* **Docker Hub**: Container Registry atau centralized storage untuk Docker Images yang dapat diakses oleh Pihak A atau Pihak B.
