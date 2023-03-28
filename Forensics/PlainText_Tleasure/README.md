# Plaintext Tleasure

## Description

Threat intelligence has found that the aliens operate through a command and control server hosted on their infrastructure. Pandora managed to penetrate their defenses and have access to their internal network. Because their server uses HTTP, Pandora captured the network traffic to steal the server's administrator credentials. Open the provided file using Wireshark, and locate the username and password of the admin.

## Solution

As always, I exported the HTTP objects from the .pcap file, using Wireshark, by File → Export Objects → HTTP.
Then I searched for ```HTB{``` in the exported files and found the flag in plain sight.

## Flag

```HTB{th3s3_4l13ns_st1ll_us3_HTTP}```