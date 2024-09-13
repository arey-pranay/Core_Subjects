#### Notes for computer networks and related concepts

youtube.com/watch?v=IPvYjXCsTg8

OSI Header 5 bytes
TCP/IP Header 20 bytes

jitter -> delay me delay

Topologies -> star, mesh, ring, bus, hybrid

Bitrate -> For efficiency of computer
Baudrate -> For transmission speed

BitRate = BaudRate * (no. of bits per baud)

Bauf -> No. of signal units per second

attenuation -> Loss in strength of signal due to resistance of medium
distortion -> Alteration of original signal induced by attenuation or noise or any other interference

Multiplexing means transmitting multiple signals through single wire
Frequency Division Multiplexing
Wavelength Division Multiplexing
Time Division Multiplexing

ARQ -> Automatic Repeat Request

Stop and Wait

Sliding Window:
    Go Back N
    Selective Repeat

MAC: Media Access Control
G -> No. of stations that wish to transmit in same time

Pure Aloha:
    Station Waits, and it is used for detecting collision
    Throughput: G * (e^-2G)
    Maximum efficiency = 18.4%.
Slotted Aloha:
    Overcome collision
     Throughput: G * (e^-G)
     Maximum efficiency = 36.8%.
     
CSMA : Carrier Sends Multiple Access

1 persistant : check if someone is sending in a time period
No persistant : check continuously
P persistant : slotted channel, probability is calculated for ideal channel situation ig
O persistant : supervisory node that forms an order to send data packet

CD : Collision Detection ( 802.3 )
CA : Collision Avoidance ( 802.11 )

Network Switching Techniques:
Circuit based
Packet based
Message based switching technique

Class A B C D E
till 127, till 191, till 223, till 239, till 255
Network Octet :  Host Octet
A B C D E
1:3, 2:2, 3:1, NA:NA, NA:NA

DHCP: Dynamic Host Configuration Protocol

IPv4 vs IPv6
Classful vs Classless
TCP vs UDP
