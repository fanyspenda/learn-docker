# Belajar Docker

## Apa itu Docker?

-   Platform untuk membungkus aplikasi kita dan menjalankannya pada suatu environment yang terisolasi, yang disebut `container`.

> **Note:**
>
> Secara simple, dapat disimpulkan bahwa **Docker mirip seperti virtual machine**, tapi untuk aplikasi kita saja, bukan OS.

## Kenapa pakai Docker?

-   (?)Jika terjadi perubahan ketika aplikasi kita sudah dideploy di production, kita bisa melakukan perubahan di production tanpa merusak apa yang ada di production tersebut dengan cara mengubahnya di container.

## Cara kembangkan aplikasi dengan Docker (Docker Life-cycle)

1. Lakukan pengembangan dan testing di container.
2. Jika sudah, deploy ke _production environment_.

## Bagaimana Cara Pake Docker?

1. tambahkan `Dockerfile` di project kita
2. isi Dockerfile. Panduan untuk frontend (Next.js) dapat dilihat di [sini](https://medium.com/@khwsc1/a-simple-react-next-js-app-development-on-docker-6f0bd3f78c2c).

> note:
>
> Tujuan dari `Dockerfile` adalah membuat suatu image file (blueprint) dengan cara mengkopi beberapa source code project kita, kemudian menginstall dependensi yang dibutuhkan.

3. Build Dockerfile dengan menjalankan perintah `docker build`. Referensi bisa dilihat di [sini](https://docs.docker.com/engine/reference/commandline/build/).
4. Setelah sukses, maka suatu imagefile akan terbentuk. periksa dengan memasukkan perintah `docker images` atau `docker images ls -a` untuk melihat keseluruhan image file yang sudah dibuat.
5. Buat suatu container (instansiasi dari image file) dengan cara `docker run`. Referensi bisa dilihat di [sini](https://docs.docker.com/engine/reference/run/).
6. Container akan dibuat dan otomatis berjalan.
7. jalankan `docker stop` untuk menghentikan container tanpa menghapusnya atau jalankan `docker rm` untuk menghentikan dan menghapus container.

## Docker-Compose

-   Menjalankan banyak container sekaligus.
-   YAML untuk konfigurasi.

## Kekurangan Docker (So far)

1. makan tempat di harddisk karena adanya imagefile dan container(?).
