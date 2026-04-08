
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

### **Step 1: Access Lima Charlie and Install the Atomic Red Plugin**

Continue where we left off in Part 1, logged into the **Lima Charlie** web interface.

Go to the **"Add-ons"** tab in the top right of the web page:

<img width="1777" height="781" alt="image" src="https://github.com/user-attachments/assets/b4d2e7c4-1c69-4201-a08f-d4dd4da0aa87" />


Scroll to find the **Atomic Red plugin** and click on **"ext-atomic-red-team"**:

<img width="1789" height="843" alt="image" src="https://github.com/user-attachments/assets/177c7a29-a56e-4b29-9c88-6ee256dd2a2d" />


Take a moment to explore other plugins and features Lima Charlie offers.

Click **"Subscribe"** on the right-hand side to install the plugin:

<img width="1423" height="750" alt="image" src="https://github.com/user-attachments/assets/15cca11f-1bea-43b2-bf8d-87d78aee3d57" />

---
### **Step2: Add Detection Rules**

Now that our sensor and add-on are set up, we need to add the **detection rules** that get triggered when running tests. 

After subscribing, return to your organization and select your machine:

<img width="1830" height="665" alt="image" src="https://github.com/user-attachments/assets/09327ddb-48cb-4682-9802-580b8893ad0e" />
<img width="1816" height="590" alt="image" src="https://github.com/user-attachments/assets/66e1dfab-34cc-4ca7-b221-c29332addcf5" />

Click on the **"Detections"** tab:
<img width="1827" height="782" alt="image" src="https://github.com/user-attachments/assets/8c13a3b5-16e3-4d99-a019-7cbcfc516e66" />


In order to select sigma rules, click on **"View extension"** in the **"ext-sigma"** tab: 
<img width="1841" height="811" alt="image" src="https://github.com/user-attachments/assets/c66cf2a8-fb59-40d9-aaef-37ec72011887" />

Click **"Subscribe"**.
<img width="900" height="708" alt="image" src="https://github.com/user-attachments/assets/49b156ef-8773-42c0-a904-610ea3a580f4" />

>[!Tip]
>
>- Sigma rules serve as the industry standard for vendor-neutral threat detection. Soteria, by contrast, is a high-fidelity managed rule set designed by security experts to offer professional-grade protection, though it typically operates as a paid service.
>
>- While these pre-packaged solutions provide excellent "out-of-the-box" coverage, you aren't locked behind a paywall; LimaCharlie’s allows you to create your own custom Detection & Response (D&R) rules manually to target specific suspicious behaviors or local threats at no extra charge.

---
### **Step 3: Run Atomic Red Tests**


In the left menu, click on **"Extensions"** and and then select **"Atomic Red Team"**:

<img width="1795" height="872" alt="image" src="https://github.com/user-attachments/assets/048dc24b-fca5-48f7-a32f-5013bb15d1df" />


From the top dropdown menu, select **your device**:

<img width="1436" height="694" alt="image" src="https://github.com/user-attachments/assets/65be4459-a0c6-4476-b474-0676678ca77a" />

Click **"Prepare Host"**.

<img width="1356" height="304" alt="image" src="https://github.com/user-attachments/assets/ba3f2dc7-6797-4b49-a632-72cc3698de03" />

Click on the **"Run tests"** section to find the **command-and-control** category.

<img width="1395" height="675" alt="image" src="https://github.com/user-attachments/assets/ecfdd703-1857-4197-9ca8-40eb7906ce4f" />

Check the box next to the category header to select all sub-tests.


Select your host again and click **"Run Tests"**:

<img width="1819" height="896" alt="image" src="https://github.com/user-attachments/assets/9d6f4dbf-6134-40af-8886-57d37e5fd1db" />

Immediately, a **"Request Success"** pop-up should appear, as well as a **"Job ID"**:

<img width="1237" height="480" alt="image" src="https://github.com/user-attachments/assets/8e128745-7e9a-4ba5-a9e1-e70bd1f03bac" />

---
### **Step 4: Analyze the Logs**



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
