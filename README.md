# Tutorial 10 - Broadcast Chat

#### Raquel Nayyara Aulia - 2206826583

## Original code, and how it run
![Original code, and how it run](assets/images/Original%20code,%20and%20how%20it%20run.jpg)

Untuk menjalankan: Ketikkan perintah `cargo run --bin server` untuk mengaktifkan server. Ketikkan `cargo run --bin client` untuk memulai klien

Ketika klien mengirimkan pesan, server akan menerima pesan tersebut, menampilkannya di terminal server, dan kemudian menyiarkan pesan itu ke klien lain yang terhubung dengan server

## Modifying port
![Modifying port](assets/images/Client.jpg)

Untuk mengubah port klien, perlu dilakukan pengubahan pada metode `ClientBuilder::from_uri()`.

![Modifying port](assets/images/Server.jpg)

Untuk mengubah port server, perlu dilakukan pengubahan pada metode `TcpListener::bind()`.

## Small changes. Add some information to client
![Small changes. Add some information to client](assets/images/Small%20changes.%20Add%20some%20information%20to%20client.jpg)

Perubahan pada `client.rs`
![Small changes. Add some information to client](assets/images/Client2.jpg)

Saya hanya menambahkan text `Raquel's Computer`

Perubahan pada `server.rs`
![Small changes. Add some information to server](assets/images/Server2.jpg)

Menambahkan client address pada pesan yang dikirim client