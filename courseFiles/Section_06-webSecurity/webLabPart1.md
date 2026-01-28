# For the Windows/Ubuntu VM

## The objective for this lab is to
- Understand how SQL Injection works
- See how it appears in logs
- See the mitigation ( how a SOC analyst should react )
- See the difference between vulnerable and secure code

## Setup

- Open **Command Prompt**

<img width="85" height="103" alt="image" src="https://github.com/user-attachments/assets/b2c7dbad-d57b-40d0-9318-ca8d40176c22" />

- Get the IP of the other VM
```bash
tailscale status
```

<img width="740" height="75" alt="image" src="https://github.com/user-attachments/assets/8ec3aa43-15fc-4a2c-a1e4-5e0caa219ef5" />

>[!IMPORTANT]
>We are looking for the **linux** VM, so grab the IP from the **linux** line
>
>For us it is `100.116.161.87`, **YOUR IP MAY BE DIFFERENT, USE YOURS**

- **SSH** into that machine
```bash
ssh ubuntu@100.116.161.87
```

Password is `metarange`

<img width="247" height="25" alt="image" src="https://github.com/user-attachments/assets/69706053-abe6-4de7-aa48-d9fd739ec4a7" />

```bash
cd ~/SOC_Analyst_Labs/WebLab
```

```bash
source .venv/bin/activate
```
```bash
python app.py
```

<img width="660" height="288" alt="image" src="https://github.com/user-attachments/assets/5cd1297e-f75d-4124-b7b4-86bb1ca403bf" />

To connect to the site open ``http://10.10.119.212:8000`` **NOTE THAT YOUR IP MAY BE DIFFERENT**

## Go to [Part 2](/courseFiles/Section_06-webSecurity/webLabPart2.md)

---
[Back to the section](/courseFiles/Section_06-webSecurity/webSecurity.md)
