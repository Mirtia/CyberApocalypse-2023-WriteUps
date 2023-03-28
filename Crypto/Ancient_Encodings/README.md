# Ancient Encodings

## Description

Your initialization sequence requires loading various programs to gain the necessary knowledge and skills for your journey. Your first task is to learn the ancient encodings used by the aliens in their communication.

## Solution

To get the decoded string from the given encoded sequence, we simply decode the string from base64
```0x53465243657a467558336b7764584a66616a4231636d347a655639354d48566664326b786246397a5a544e66644767784e56396c626d4d775a4446755a334e665a58597a636e6c33614756794d33303d```

```python
from Crypto.Util.number import long_to_bytes
from base64 import b64decode

def decode(message):
    return b64decode(long_to_bytes(int(message, 16)))

message = "0x53465243657a467558336b7764584a66616a4231636d347a655639354d48566664326b786246397a5a544e66644767784e56396c626d4d775a4446755a334e665a58597a636e6c33614756794d33303d"
```
## Flag

```HTB{1n_y0ur_j0urn3y_y0u_wi1l_se3_th15_enc0d1ngs_ev3rywher3}```