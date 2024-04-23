# advprog-modul8-Publisher

# Mahoga Aribowo Heryasa

# 2206025230

### How many data your publlsher program will send to the message broker in one run?

Berdasarkan program yang dijalankan pada `main.rs`, program publisher akan mengirimkan lima data ke *message broker* dalam satu kali run. Hal ini terjadi karena terdapat lima pemanggilan method `publish_event` yang pada masing-masing pemanggilannya mengirimkan `UserCreatedEventMessage` ke *message broker*.

### The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

URL `amqp://guest:guest@localhost:5672` digunakan dalam program *publisher* dan program *subscriber* untuk membangun koneksi ke server APMQ yang sama. Dengan bergitu, *publisher* dan *subscriber* akan saling melakukan komunikasi melalui *message broker* yang sama. *Publisher* akan mengirim pesan dan *subscriber* yang terhubung ke akan menerima pesan tersebut.

### Running RabbitMQ as message broker:

![Running RabbitMQ as message broker](assets/images/RunningRabbitMQ.png)