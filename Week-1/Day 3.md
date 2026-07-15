**DAY 3**
Yesterday I learned:
"How do computers find each other?" → IP addresses (Layer 3)
Today I'll learn:
Once two computers know each other's address, how do they actually communicate?" → TCP/UDP and Ports (Layer 4)
-Here is what will happen when u search something on Internet:

You
 │
 │  "Open YouTube"
 ▼
Application Layer
 │
 │  "Use HTTPS"
 ▼
Transport Layer
 │
 │  "I'll use TCP"
 ▼
Network Layer
 │
 │  "Google's IP is 142.x.x.x"
 ▼
Internet

-Let's say Google is big company.You know the destination point is in google, but u don't have info anbout who is responsible to get that request(message)
-To add that employye addresss into your mailing address, they make sth new called **PORT.**.

-Port number identifies a specific network service or application running on a computer. While the IP address tells data which computer to reach, the port number tells the operating system which application should receive that data. Together, they form a socket address, such as 192.168.1.10:443.

**COMMON PORTS**

|    Port | Protocol | Purpose                              | Typical Use               |
| ------: | -------- | ------------------------------------ | ------------------------- |
|  **22** | SSH      | Secure remote login                  | Manage Linux servers      |
|  **53** | DNS      | Convert domain names to IP addresses | Website lookups           |
|  **80** | HTTP     | Unencrypted web traffic              | Basic websites, redirects |
| **443** | HTTPS    | Encrypted web traffic                | Secure websites and APIs  |

**TCP(Transmission Control Proocol)**: always want to send full package,if something is missing it return the packets to be sent again.such as Web browsing (HTTP/HTTPS),SSH (port 22),Email, File transfers(in short it is Reability checker)
**UDP(Use Data Protocol)**: always care about the speed.we use this for videocalls and streaming.it doesn't care if some packets r not fully delivered or not.
-200 → OK
-404 → Not Found
-403 → Forbidden
-500 → Server Error

when we type this curl -v http://example.com on our terminal it show us what is happening between in our machine and the server we wan to connect.

cat /etc/services | head -n 20

- **cat** means show me what is inside this file.
- **/etc/services**   is a file that contains a list of: Service names, Port numbers, Protocols (TCP/UDP)








