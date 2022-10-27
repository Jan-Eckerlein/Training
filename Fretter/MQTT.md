## Aufgabe 2

Beschreiben Sie den Ablauf der MQTT-Kommunikation, der durch die folgende Abbildung dargestellt wird.

![](C:\Users\janec\AppData\Roaming\marktext\images\2022-10-27-12-31-54-image.png)



### Lösung:

- Client A verbindet sich mit dem Broker

- Client B Published ein Paket im ``temperature/roof``

- Client A abboniert dieses Topic und bekommt direkt das erste Paket dazu von dem Broker

- Client A published ein Paket im ``temperature/floor``

- Client B Published ein Paket im `temperature/roof`, was der Broker an Client A schickt.

- Client A bricht die Verbindung mit dem Broker ab


