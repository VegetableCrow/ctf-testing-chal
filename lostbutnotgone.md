2nd Forensic challenge given by CoffeeSoDa, we are given an ad1 file.

Open it using FTK Imager, since the name of this chal is Lost But Not Gone, I checked the RecycleBin first.

![image](https://github.com/user-attachments/assets/b9265838-bd09-4d16-9116-98180fafd6be)


Found a text file with the contents of, secret:bm93X2l0c190aW1lX2Zvcl9maWxlc3Nzc3Mg==

This is a Base64 code, so decode it and you will get, now_its_time_for_filesssss
![image](https://github.com/user-attachments/assets/cbba987e-b6a5-4c1a-bf02-db592cdd47a9)


Found a zip file called filess.zip so I'm pretty sure the flag is in here.
![image](https://github.com/user-attachments/assets/e2348d23-c2e3-4fad-8adc-98fdae1eb6ef)

Got a bit stuck at this point but I thought "Could the secret be the password to the zip file?" 
So I exported the zip file, and voila, managed to unlock it with the secret.

![image](https://github.com/user-attachments/assets/73e8549c-173b-4915-880c-e1e1ed45b131)
![image](https://github.com/user-attachments/assets/fdb5012a-5477-43ca-ad95-2a67c1ff2c83)
![image](https://github.com/user-attachments/assets/edfc51cc-df9e-43d3-992d-07ddfe541c6c)

And then, you will get 100 of text files, the easier way is to use Linux to cat and grep,

![image](https://github.com/user-attachments/assets/d0c44913-1a42-459c-81f2-89f3caf43da1)

Or you can just view each file one by one :D (Dont be like me, i was lazy to open Kali Linux)
![image](https://github.com/user-attachments/assets/ef7ad940-bcf7-48e8-b5ff-366ccf2d3456)


Flag: TARUMT{s0_M@NY_z!p}






