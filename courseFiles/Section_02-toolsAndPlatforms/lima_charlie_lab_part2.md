
# **Lima Charlie meets Atomic Red**

---

### **Part 2 of 2**  

>[!Tip]
>
> _Please complete [Part 1](./lima_charlie_lab_part1.md) of this lab first._

---

In this lab we will be creating a **controlled and fake cyber attack** with **Atomic Red**.  
We will then use **Lima Charlie** to observe what is logged and how a real-world attack may trigger alerts for investigation.

---

### **Step 1: Access Lima Charlie**

Continue where we left off in Part 1, logged into the **Lima Charlie** web interface.

### **Step 2: Install the Atomic Red Plugin**

Go to the **"Add-ons"** tab in the top right of the web page:

<img width="1777" height="781" alt="image" src="https://github.com/user-attachments/assets/b4d2e7c4-1c69-4201-a08f-d4dd4da0aa87" />


Scroll to find the **Atomic Red plugin** and click on **"ext-atomic-red-team"**:

<img width="1789" height="843" alt="image" src="https://github.com/user-attachments/assets/177c7a29-a56e-4b29-9c88-6ee256dd2a2d" />


Take a moment to explore other plugins and features Lima Charlie offers.

Click **"Subscribe"** on the right-hand side to install the plugin:

<img width="1423" height="750" alt="image" src="https://github.com/user-attachments/assets/15cca11f-1bea-43b2-bf8d-87d78aee3d57" />

---

### **Step 3: Run Atomic Red Tests**

After installation, return to your organization and select your machine:

<img width="1830" height="665" alt="image" src="https://github.com/user-attachments/assets/09327ddb-48cb-4682-9802-580b8893ad0e" />
<img width="1816" height="590" alt="image" src="https://github.com/user-attachments/assets/66e1dfab-34cc-4ca7-b221-c29332addcf5" />


In the left menu, click on **"Extensions"** and and then select **"Atomic Red Team"**:

<img width="1795" height="872" alt="image" src="https://github.com/user-attachments/assets/048dc24b-fca5-48f7-a32f-5013bb15d1df" />


From the top dropdown menu, select **your device**:

<img width="1436" height="694" alt="image" src="https://github.com/user-attachments/assets/65be4459-a0c6-4476-b474-0676678ca77a" />

Click **"Prepare Host"**, then scroll down to find the **command-and-control** category.  
<img width="1324" height="460" alt="Screenshot from 2026-04-07 13-45-08" src="https://github.com/user-attachments/assets/b6200abd-4ba9-44d7-8f63-ab70dba4bc99" />
Check the box next to the category header to select all sub-tests.


Click **"Run Tests"**:

![](attachments/C2ALL.PNG)

---

### **Step 4: Analyze the Logs**

Switch to the **"Detections"** tab on the left:

![](attachments/detections.png)  
![](attachments/logsscreen.png)

You'll see many events. Each time the page refreshes, new attacks may appear.

Look for **cmd.exe** or **powershell** executions.  
These are often indicators of **potential malicious activity** and warrant further investigation.

![](attachments/DETECTED.PNG)

---

### **Conclusion**

**Lima Charlie** proves to be a powerful and versatile tool:  
- Simple and intuitive interface  
- Detailed forensic capabilities before, during, and after an attack  
- Scalable for both small and large organizations  
- Plugin system for extended automation and detection


---
[Back to the Section](/courseFiles/Section_02-toolsAndPlatforms/toolsAndPlatforms.md)
