5th Forensic Challenge given by CoffeeSoDa, we are given a corrupted gif file.

Judging from the name of the file, this challenge requires us to fix the magic number of the file.


> [!NOTE]
> Magic numbers are the first bits of a file which uniquely identify the type of file.
> 
> I used this website to refer [File Magic Numbers](https://gist.github.com/leommoore/f9e57ba2aa4bf197ebc5)
>
> 



The magic number for a gif file is `47 49 46 38`.

I'm using the software `HxD` for this. Open the gif file using it.
Download HxD: https://mh-nexus.de/en/downloads.php?product=HxD20

 <br> 
 <br> 

As we can see, the starting bytes are not that of a gif file, we need to change that.

![image](https://github.com/user-attachments/assets/82f843ad-a400-463e-8949-d1bb13331512)


Here is the proper magic bytes example for a gif file.

![image](https://github.com/user-attachments/assets/411c6f40-2479-45e4-a22f-a0d6cf86066b)
 <br> 
 <br> 

### **Modify the Magic Number**

First, I copied the right bytes  `47 49 46 38`, 
Then, highlight the wrong bytes `6D 61 47 69`, right click, and click `Paste Insert` .
And then, save the file.
 <br> 
![image](https://github.com/user-attachments/assets/dc24936f-50cb-4cb3-9340-74f62be32560)
![image](https://github.com/user-attachments/assets/187bfefb-df26-487e-8ece-4b02c89a6788)

 <br> 
<br> 

### **Fixed GIF File** 
And voila, the gif file is fixed. The gif file seems to be made of 2 frames.
![image](https://github.com/user-attachments/assets/d76429b7-f680-42a5-9b41-6c8d174b1f99)
![image](https://github.com/user-attachments/assets/d2a3dc4e-c7cc-47b2-be6e-69f2f84a26ac)

In the second frame, we are given a hex string.
`6d 40 47 31 43 5f 4c 75 4d 38
33 52 72 52 72 72 52 21 21 21
0d 0a`

Using a Hex to ASCII converter online, we can get the flag.
![image](https://github.com/user-attachments/assets/68f165a0-193c-494e-a7b3-a5eb45b03f2e)

**Flag:** TARUMT{m@G1C_LuM83RrRrrR!!!}










