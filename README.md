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

## Docker-Compose

-   Menjalankan banyak container sekaligus.
-   YAML untuk konfigurasi.
