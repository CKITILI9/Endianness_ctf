#ENDIANNESS CHALLENGE
- Endianness is a byte transfer procedure that explains how computers store and transmit multi-byte data.
- Byte transfer is divided into two categories: little endian and big endian
- This challenge teaches us how to find little endian and big endian using the "deogy" word
---



#Environment
- Host Machine: Windows 10 with Oracle VirtualBox
- Guest: Ubuntu 20.04 LTS (CLI-based)
- Access: SSH via PuTTY
---



#Steps Taken
- Launched the game from picoctf.
- Used netcat to access the game remotely.
- The challenge asked us to find little endian first
- So I used cyberchef, a web based platform that changes the given word, "deogy",  into hex
- The hex value for the word was: 64656f6779
- So little endian value will be the hex value, reversed: 79676f6564
- Big endian will be: 64656f6779 (the normal order)
---



#Key Takeaways
- Endianness is mostly about bytes and not letters. Computers read and process numbers.
- Hex values let us read binary in an easy way.
- The challenge connected the dots between: text, hex values, and byte order.
