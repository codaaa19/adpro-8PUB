## QUESTION ADPRO 8

1. How many data your publlsher program will send to the message broker in one run?

Setiap pemanggilan function publish_event() akan mengirimkan 1 pesan ke broker dan 5 ke program utama. Maka tiap esekusi akan mengirimkan 5 pesan.

2. The url of: `amqp://guest:guest@localhost:5672` is the same as in the subscriber program, what does it mean?

Hal ini memastikan bahwa subscriber dan publisher terhubung pada infrastruktur pesan yang sama agar dapat bertukar pesan secara lancar.

## RABBITMQ

![alt text](image.png)

![alt text](image-1.png)

Publisher akan mengirimkan pesan data, yaitu 5 event kepada subscriber

![alt text](image-2.png)

Grafik spike berikut dipengaruhi oleh esekusi publisher. Semakin banyak jumlah pesan dalam queue, semakin besar juga lonjakannya