3rd Forensic challenge given by CoffeeSoDa, we are given a jpg file called stegORForensic.jpg
<br>

## **First Image: stegORForensic.jpg**
![image](https://github.com/user-attachments/assets/bc061876-f218-4279-b06d-a435017b0102)

<br>

Tried file and exiftool, nothing seems out of the ordinary.
![image](https://github.com/user-attachments/assets/1fefc5fd-9880-46d2-8611-41af6818bd62)

<br>
So, I tried using the command steghide to see if I can extract anything. Since we dont have any passphrase, just leave it blank and press Enter.

![image](https://github.com/user-attachments/assets/c6efa197-97dd-4d61-abbc-327f801f0850)


We got another jpeg file from that.

![image](https://github.com/user-attachments/assets/6e31b131-d124-436b-8dab-8070c213c75c)

<br>
<br>

## **Second Image: isThisHowUThoughtUr.jpeg**
Exiftool the image file,

![image](https://github.com/user-attachments/assets/9df3fce2-bd8f-4579-8ad1-7da9ce7d44f9)

We got the comment of `stegsteg`, I figured this might the passphrase to steghide it.

So now, we steghide the `isThisHowUThoughtUr.jpeg` with the passphrase `stegsteg`, and we will get a text file
![image](https://github.com/user-attachments/assets/02118fb6-5e7d-4fb9-ad6b-9cdc02440ebd)


Open the text file, and we get the flag.

![image](https://github.com/user-attachments/assets/0b60eeb8-1791-40eb-bf6f-ddac77a41d9d)

**Flag:** TARUMT{WAiT?ST3g_!$_F0r3N$1c?}












