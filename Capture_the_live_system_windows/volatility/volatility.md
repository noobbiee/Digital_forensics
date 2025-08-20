# Windows Info

At first we will try gather all information about the windows versions and other basic info we can gather about the memory dump

<img width="893" height="431" alt="Screenshot from 2025-08-19 15-39-19" src="https://github.com/user-attachments/assets/1699c7d2-b9de-47e3-9e09-1508ea7c2382" />

<img width="893" height="431" alt="Screenshot from 2025-08-19 15-39-34" src="https://github.com/user-attachments/assets/5d192dbc-4daf-485b-bc18-6842a1bd2a3e" />

We found the memory location where the kernel is loaded. It also confirms dump is from 64Bit windowsOS, withIntel processor and has 4 processor. It confirms it is windows version 10, we can see the date and timestamp at which the dump was taken.

# Processes list

We can check all the process that were running during the time of the memory dump

<img width="884" height="484" alt="Screenshot from 2025-08-19 16-22-13" src="https://github.com/user-attachments/assets/59f5784c-9d41-4b4f-b177-b97e7c120353" />

<img width="884" height="484" alt="Screenshot from 2025-08-19 16-22-26" src="https://github.com/user-attachments/assets/85c20ef7-1a1d-4327-9691-a910c2e14b29" />

# Malfind

We can run the dump and try to find the malware, it has the hashes of the known malware and tries to match the hash to find malwares.

<img width="896" height="398" alt="Screenshot from 2025-08-19 16-38-49" src="https://github.com/user-attachments/assets/40eada54-79f8-4265-bff1-4266d3523e1f" />

<img width="896" height="398" alt="Screenshot from 2025-08-19 16-39-03" src="https://github.com/user-attachments/assets/0f0a9c35-96dc-4216-a80d-42551b2b0f45" />

<img width="891" height="446" alt="Screenshot from 2025-08-19 16-39-15" src="https://github.com/user-attachments/assets/f25de026-f23e-4221-bb09-80db8bcf9e2f" />

It says that there are two malware on Searchapp.exe on process 5960. It is giving us the hex of the file and assembly codes.

# Process tree

We can see the all process running along with the child process on the system

<img width="954" height="646" alt="Screenshot from 2025-08-19 16-45-21" src="https://github.com/user-attachments/assets/f3c44071-35e4-4045-ae38-2d2f55429d72" />

<img width="1139" height="719" alt="Screenshot from 2025-08-19 16-45-44" src="https://github.com/user-attachments/assets/a04aac39-7254-494f-9bb5-b9da4b9e448a" />

This is the process that was determined malicious by the malfind. 

<img width="925" height="697" alt="Screenshot from 2025-08-19 16-49-14" src="https://github.com/user-attachments/assets/d284e92a-a2eb-4f0f-8551-babfbbedb382" />

# Memmory map

We can view the entire memorymap

<img width="697" height="638" alt="Screenshot from 2025-08-19 16-59-21" src="https://github.com/user-attachments/assets/e3353941-b690-4b8b-830b-72cdb18cd0b2" />

# windows registry hivelist

We can see the registry in the memory dump that we captured. 

<img width="896" height="474" alt="Screenshot from 2025-08-19 18-45-00" src="https://github.com/user-attachments/assets/8808ba21-3e86-4454-8d6d-12545209c784" />

<img width="898" height="205" alt="Screenshot from 2025-08-19 18-45-29" src="https://github.com/user-attachments/assets/fab9b4b2-0262-4c15-a31c-ecbd424195eb" />

# certificates

We can check all the certifiactes that were in memeory during dump.

<img width="893" height="420" alt="Screenshot from 2025-08-20 10-32-24" src="https://github.com/user-attachments/assets/617e937d-c773-478a-8a34-49dd71ed8182" />

<img width="887" height="443" alt="Screenshot from 2025-08-20 10-32-34" src="https://github.com/user-attachments/assets/b4653350-9187-4454-a388-217651b65767" />

<img width="887" height="443" alt="Screenshot from 2025-08-20 10-32-44" src="https://github.com/user-attachments/assets/c0e6a465-d821-4828-b87d-e4abc3f325ee" />






