# Embedded Communication Protocols Notes

## OSI Model Layers
```
+------------+--------------+--------------------------+--------------------------+ 
|						LAYER						   | Protocol Data Unit (PDU) |
+------------+--------------+-----+--------------------+--------------------------+
| 			 | 				| [7] | Application layer  | 						  | 
+ 			 |				+-----+--------------------+						  +
| 			 | 				| [6] | Presentation layer | 		   DATA		      |
+ High Layer | Application  +-----+--------------------+						  +
| 			 |	Layer	    | [5] |	Session layer	   |						  |
+			 +--------------+-----+--------------------+--------------------------+
| 			 | 				| [4] |	Transport layer    | 	 Segment, datagram    |
+------------|				+-----+--------------------+--------------------------+
|			 | 				| [3] |	Network layer	   |	    Packet			  |
+		 	 |	Data flow	+-----+--------------------+--------------------------+
| HW Layer	 |	Layer		| [2] | Data link layer    | 		Frame			  |
+ 			 |				+-----+--------------------+--------------------------+
| 			 | 				| [1] |	Physical layer     |	 	Bit, Symbol		  |
+------------+--------------+-----+--------------------+--------------------------+

```
### Description
- [7]. **Application layer:**High-level protocols such as for resource sharing or remote file access, e.g. HTTP	
- [6]. **Presentation layer:** Translation of data between a networking service and an application; including character encoding, data compression and encryption/decryption
- [5]. **Session layer:** 	Managing communication sessions, i.e., continuous exchange of information in the form of multiple back-and-forth transmissions between two nodes
- [4]. **Transport layer:** Reliable transmission of data segments between points on a network, including segmentation, acknowledgement and multiplexing
- [3]. **Network layer:** Structuring and managing a multi-node network, including addressing, routing and traffic control
- [2]. **Data link layer:** Transmission of data frames between two nodes connected by a physical layer
- [1]. **Physical layer:**  Transmission and reception of raw bit streams over a physical medium
                                                 
## List of communication protocols

- SPI/QSPI
- I2C
- UART/USART
- BLUETHOOT
- USB
- ETHERNET
- CAN/CANFD
- FLEXRAY

STANDARDs
- J1939
- ISO 11898

## References 

- OSI Model: https://en.wikipedia.org/wiki/OSI_model
- Communication Protocols: https://en.wikipedia.org/wiki/Communication_protocol#Layering
Science direct/Demystifying Embedded Systems Middleware, 2010: https://www.sciencedirect.com/topics/engineering/embedded-system-model#:~:text=OSI%20Model%20Layer%201%3A%20Physical,see%20Figure%202%2D28)
- Pubnub: https://www.pubnub.com/learn/glossary/communication-protocols/
