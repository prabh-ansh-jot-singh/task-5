# Wireshark Network Traffic Capture

## Objective
Capture live network packets and identify basic protocols and traffic types using Wireshark.

## Steps Taken
1. Installed Wireshark and started capturing on the active network interface.
2. Browsed websites and pinged `google.com` to generate traffic.
3. Filtered packets by protocols: HTTP, DNS, TCP.
4. Stopped capture after 1 minute and exported as `.pcap` file.

## Protocols Identified
1. **TCP** - Transmission Control Protocol, used for reliable data transfer.
2. **UDP** - User Datagram Protocol, used for fast, connectionless communication.
3. **DNS** - Domain Name System, used for resolving domain names to IP addresses.
4. **HTTP** - Hypertext Transfer Protocol, used for browsing web pages.

## Sample Packet Details
| No | Source IP       | Destination IP | Protocol | Info                        |
|----|----------------|----------------|---------|----------------------------|
| 1  | 192.168.0.101  | 142.250.190.78 | TCP     | TCP handshake              |
| 2  | 192.168.0.101  | 8.8.8.8        | DNS     | Standard query A google.com|
| 3  | 192.168.0.101  | 142.250.190.78 | HTTP    | GET /                       |

## Conclusion
Captured network traffic shows multiple protocols in action. Wireshark helps in analyzing packet flow, troubleshooting network issues, and understanding protocol behavior.

## Files
- `network_capture.pcap` → Packet capture file
- `README.md` → Summary report
