## Aufgabe 2:

1. Beschreiben sie das prinzipielle Funktionsprinzip von MQTT
   
   - Mit **MQTT**  werden Nachrichten über einen Broker mit anderen Geräten oder Software geteilt. Jede Nachricht verfügt über ein Topic, anhand dessen die Nachricht vom Broker weiterverarbeitet werden kann. Zusätzlich verfügt jede Nachricht über einen Nachrichteninhalt, die sogenannte Payload.

2. Unterschied zw. Qos 0, Qos 1 und Qos 2, (Qos  = Quality of Service)
   
   - 0 - at most once
     
     - Der Kunde veröffentlicht die Nachricht einfach, und es erfolgt keine Bestätigung durch den Broker.
   
   - 1 - at least once
     
     - garantiert, dass die Nachricht erfolgreich an den Broker übermittelt wird
     
     - Der Broker sendet eine Bestätigung an den Absender zurück
     
     - Wenn die Bestätigung nicht beim Absender ankommt, weis dieser nicht, dass die Urspüngliche Nachricht angekommen ist und sendet erneut
     
     - --> garantiert ankommen, kann allerdings mehrfach beim Broker ankommen
   
   - 2 - exactly once
     
     - Folge von vier Nachrichten zwischen Absender und Broker
     
     - Bei einem Handschlag wird sowohl dem Absender bestätigt, dass die Nachricht angekommen ist, als auch dem Broker, dass der Empfänger die Bestätigung erhalten hat

3. Beispiele:
   
   -  
