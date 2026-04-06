
# **LimaCharlie Lab**

---

## **Part 1 of 2 – Endpoint Monitoring & Threat Detection**

In this lab we will be using **LimaCharlie** to investigate **endpoint monitoring** and **threat detection**.

### **What is LimaCharlie?**

LimaCharlie is a lightweight browser-based tool. It helps monitor systems, detect threats, and respond quickly to suspicious activity. This walkthrough uses the **Chrome** browser, but any browser may be used.

---

## **Step 1: Access LimaCharlie and sign up**

Open a browser and go to:

```
https://app.limacharlie.io/
```

Click **"Sign up"**:

<img width="601" height="545" alt="image" src="https://github.com/user-attachments/assets/0bc77d14-d6c2-4251-bb28-b422f8be6791" />

Fill out the required field and press **"Continue"**, then press **"Add Password"**: 

<img width="615" height="723" alt="image" src="https://github.com/user-attachments/assets/a7d95916-deca-48ed-a6b6-5882b96442d4" />

Fill out the required fields and click **"Sign Up"**.

<img width="627" height="794" alt="image" src="https://github.com/user-attachments/assets/03457146-3649-4647-83f6-b626d690a812" />


Check your email, click the verification link, then return to your browser and refresh the page.

---

## **Step 2: Setup Company Information**

You will be asked questions about your company. Use fictional information.

Enter the following details:

- **What best describes your team/company?** → *Security Operations Center*
- **What best describes your role?** → *Security Engineer*
- **What use cases are you exploring?** → *Endpoint Detection & Response*
- **How did you hear about us?** → *Black Hills Info Sec*

<img width="850" height="860" alt="image" src="https://github.com/user-attachments/assets/c4cc2950-f437-454c-be1f-d69bd99b462d" />


Check the box to agree to the Terms of Service and Privacy Policy.

Click **"Got it"** then **"New Organization"**.

<img width="726" height="355" alt="image" src="https://github.com/user-attachments/assets/61743688-e46a-49bd-97a7-7c5dcd97f008" />

# An Overview of LimaCharlie.

Before you get set up, here's the basics:

* *Sensors* are the primary input for data into LimaCharlie. They run on a variety of supported platforms and send JSON events to LimaCharlie's cloud in real-time. Embedded platforms (e.g. Windows, Mac, Linux) expose deeper capabilities like sending commands and collecting artifacts.
* *Organizations* are akin to “projects” - they're located in a chosen region and are where configuration and storage is located for a fleet of Sensors and their accompanying infrastructure.
* *Outputs* allow you to forward your data to storage only you control — like an SFTP server or Amazon S3. Storage within LimaCharlie is optional and allows you to store artifacts (i.e. logs) as well as search, browse, and replay historical Sensor data.
* *Add-ons* let you enable features within organizations à la carte, allowing you to run each org as lean or as sophisticated as your needs require.

The first step is to create an organization.


Fill out your fictional organization’s details.

<img width="899" height="661" alt="image" src="https://github.com/user-attachments/assets/d1aceb8e-ba05-4681-8a7e-d979f5324a3d" />


Click **"Create Organization"**.

Wait for the organization to be created. To check, go to **"Organizations"**: 

<img width="1811" height="471" alt="image" src="https://github.com/user-attachments/assets/27667ac6-3a9a-4de8-a6fd-ce40988814f1" />


Select your organization to continue.

---

## **Step 3: Create a Sensor**

Under the left-hand menu, go to **Sensors → Installation Keys**.

![](attachments/one.PNG)

Click **"Create Installation Key"**.

![](attachments/two.PNG)

Fill in a description and tags, then click **"Create"**.

![](attachments/three.PNG)

Next, go to **Sensors List**.

![](attachments/four.PNG)

Click **"Add Sensor"**.

![](attachments/addsensor.png)

Scroll down and select the **Windows** sensor.

![](attachments/five.PNG)

From the drop-down, select the installation key created earlier and click **"Select"**.

![](attachments/six.PNG)

Choose the architecture: **"86-64 exe"**.

![](attachments/seven.PNG)

Click **"Download the selected installer"**.

Copy the command string from **Step 4**.

![](attachments/eight.PNG)

---

## **Step 4: Install the Sensor**

Go to your desktop, right-click **Windows Terminal**, and select **"Run as administrator"**.

![](attachments/nine.PNG)

Navigate to your Downloads directory:

```
cd .\Downloads
```

Begin typing the following command and use **Tab** for auto-completion:

```
.\hcp_win_x64_release_4.29.2.exe
```

Paste the copied command string and press **Enter**.

If successful, your output will look like this:

![](attachments/correctoutput.png)

Return to your browser. You should see a confirmation message:

![](attachments/success.PNG)

>[!TIP]
>
> **Note**: Your computer name will differ.

---

## **Next Steps**

- [Continue to Part 2 of the Lab](./lima_charlie_lab_part2.md)


>[!IMPORTANT]
>
> **Important**: Always destroy your lab environment after completing exercises.

---
[Back to the Section](/courseFiles/Section_02-toolsAndPlatforms/toolsAndPlatforms.md)
