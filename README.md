# Day-5-ElevateLabs-Internship


Wireshark Packet Capture Summary

Filtering by protocol revealed active usage of:

   1. DNS for domain resolution

   2.TCP for establishing and maintaining connections

   3. TLSv1.3 for encrypted communication (HTTPS)

Notable traffic involved requests to Google services, GitHub, and certificate authorities. A typical TCP 3-way handshake was observed followed by TLS negotiation. DNS queries returned both A (IPv4) and AAAA (IPv6) records.

Some TCP sessions were closed using RST flags, possibly indicating rejected or abruptly ended connections. No malicious patterns were identified in the visible capture, though deeper inspection with filters could be done for threat hunting.





📌 General Summary

   1. Total Packets: 3620 (see bottom status bar)

  Source IPs:

  Internal (e.g., 192.168.1.17, my device)

  External services (e.g., 20.207.73.82, 142.250.183.130)

   2. Common Destinations:

        Google domains (play.google.com, gstatic.com, clients6.google.com)

        GitHub (github.com)

        OCSP responders (for certificate checking)

