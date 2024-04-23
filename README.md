1. How many data your publlsher program will send to the message broker in one run?  

Publisher akan mengirimkan lima pesan data ke broker pesan dalam satu kali eksekusi. Setiap panggilan ke publish_event akan mengirimkan satu UserCreatedEventMessage ke antrian "user_created".

2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 

URL "amqp://guest:guest@localhost:5672" merupakan URL koneksi ke server AMQP (RabbitMQ) dengan kredensial default (nama pengguna: guest, kata sandi: guest) yang berjalan pada localhost dengan port 5672. Artinya baik publisher maupun subscriber akan terhubung ke RabbitMQ yang sama menggunakan kredensial dan alamat yang sama untuk komunikasi.


Opening RabbitMQ in http://localhost:15672 
![Running RabbitMQ](img/running-rabbitmq.png)

Sending and processing event.
![Sending and processing event.](img/sending-and-processing-event.png)