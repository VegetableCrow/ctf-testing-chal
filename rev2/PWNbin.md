
![image](https://github.com/user-attachments/assets/e3f38d24-6ca3-4c8f-a27f-b65659ea09b4)

After run the chal, it outputs nothing informative

![image](https://github.com/user-attachments/assets/5bf2c30b-72bf-4e2b-9f9f-d6ed2794e78f)

Looking into the code with ghidra, the condition make it the printf function will display the flag when the local_c = 0.
We will edit the local_c value to 0 from 1 then we export the file and run again.

![image](https://github.com/user-attachments/assets/127b9c82-6ca6-4983-ab5f-0bda5830e2fc)

Run file again and the flag will be display in a base 64 string.

![image](https://github.com/user-attachments/assets/8d32584a-c6a9-471f-87f2-ca77377ca7a4)
Convert it into string and get the flag.

**FLAG**
TARUMT{St@T!c_MaKE_l!FE_eZ}
