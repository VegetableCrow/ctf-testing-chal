2nd Forensic challenge given by CoffeeSoDa, we are given an ad1 file.

> [!NOTE]
> I recommend this blog if you are learning forensics, helps a lot :D
> 
> https://zach-wong.gitbook.io/easy-reads/forensics-ctf-methodology/hard-disk-analysis-methodology
>
> 

<br>
<br>

### **Open it using FTK Imager**
Since the name of this challenge is Lost But Not Gone, I checked the RecycleBin first.

![image](https://github.com/user-attachments/assets/c83e2adf-50ca-4f8f-a6be-b1d9c0b0d43c)


Found a text file with the contents of, `secret:bm93X2l0c190aW1lX2Zvcl9maWxlc3Nzc3Mg==` .

<br>
<br>

### **Secret Base64 Decode**
This is a Base64 code, so decode it and you will get, now_its_time_for_filesssss
![image](https://github.com/user-attachments/assets/cbba987e-b6a5-4c1a-bf02-db592cdd47a9)


That is not the flag so we need to look elsewhere now.

Found a zip file called filess.zip so I'm pretty sure the flag is in here.
![image](https://github.com/user-attachments/assets/e2348d23-c2e3-4fad-8adc-98fdae1eb6ef)

However all the text files are unreadable.
![image](https://github.com/user-attachments/assets/ff2fca4d-5f4a-4fdc-9ddf-33b8a1274ff4)

<br>
<br>

### **Unzipping Zip File** 

Got a bit stuck at this point but I thought "Could the secret be the password to the zip file?" 
So I exported the zip file, and voila, managed to unlock it with the secret.

![image](https://github.com/user-attachments/assets/73e8549c-173b-4915-880c-e1e1ed45b131)
![image](https://github.com/user-attachments/assets/fdb5012a-5477-43ca-ad95-2a67c1ff2c83)
![image](https://github.com/user-attachments/assets/edfc51cc-df9e-43d3-992d-07ddfe541c6c)

<br>
<br>

### **Finding The Flag** 
**1) The easier way is to use Linux to cat and grep,**

![image](https://github.com/user-attachments/assets/d0c44913-1a42-459c-81f2-89f3caf43da1)

<br>

**2) Another good way is by identifying the last modified date or time, or size of the file.**
   
In this case, all the files have the same size of 1KB.

![image](https://github.com/user-attachments/assets/e5d51dee-bb10-402b-bce2-d03beda1149e)

However, there is one file that has a different last modified time.
![image](https://github.com/user-attachments/assets/739e19d7-d6ba-4d6b-824d-563878dd30e3)

<br>


**3) Or you can just view each file one by one :D (Dont be like me, i was lazy to open Kali Linux)**
![image](https://github.com/user-attachments/assets/ef7ad940-bcf7-48e8-b5ff-366ccf2d3456)


**Flag:** TARUMT{s0_M@NY_z!p}






