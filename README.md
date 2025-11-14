# 🧑‍💻 Phishing Simulation & Awareness Training

[Live Preview](https://svengeurtsen.github.io/phishing-simulation/)

## 🎯 Objective
The goal of this project was to assess how vulnerable employees are to phishing attacks and social engineering tactics.  
A realistic phishing campaign was conducted against a small group of test users within a real organization to evaluate their response to deceptive emails and fake login portals.  
Following the test, an awareness training was provided to improve the organization’s overall phishing resilience.

---

## 🧩 Project Overview
I independently designed and launched a complete phishing simulation.
I created a convincing email claiming there had been a “suspicious login attempt” and instructing employees to reset their password through a provided link.
This link directed them to a cloned login page of the organization’s internal Report App, which I fully built myself. Submitted credentials were securely captured on my custom backend server.

To demonstrate real-world data exfiltration, the captured credentials were forwarded through an encrypted Discord bot integration.
After submitting information, users were redirected to a custom awareness landing page explaining that this was part of a controlled security assessment.

---

## 🧠 Skills Learned
- Designing and executing phishing simulations safely and ethically  
- Applying social engineering principles in realistic testing scenarios  
- Building and hosting cloned phishing pages with HTML, SSL, and domains  
- Setting up servers for secure credential capture and validation  
- Tracking user behavior via analytics tools  
- Developing and delivering security awareness training  

---

## 🧰 Tools Used
<div>
<img src="https://img.shields.io/badge/-HTML5-E34F26?&style=for-the-badge&logo=HTML5&logoColor=white" />
<img src="https://img.shields.io/badge/-DreamHost-0073CF?&style=for-the-badge&logoColor=white" />
<img src="https://img.shields.io/badge/-FileZilla-BF0000?&style=for-the-badge&logo=FileZilla&logoColor=white" />
<img src="https://img.shields.io/badge/-Google_Analytics-F9AB00?&style=for-the-badge&logo=GoogleAnalytics&logoColor=white" />
<img src="https://img.shields.io/badge/-Discord_Bot-5865F2?&style=for-the-badge&logo=Discord&logoColor=white" />
<img src="https://img.shields.io/badge/-Curl-073551?&style=for-the-badge&logo=curl&logoColor=white" />
<img src="https://img.shields.io/badge/-Python_Server-3776AB?&style=for-the-badge&logo=Python&logoColor=white" />
</div>

---

## ⚙️ Steps

### 1️⃣ Phishing Email Creation
A convincing phishing email was crafted and sent to five employees.  
It simulated a legitimate internal security message with a link to a cloned login portal.

### 2️⃣ Fake Login Pages
Three HTML pages were created and hosted:
- **index.html** — fake login page  
- **pass.html** — password reset prompt  
- **awareness.html** — educational page shown after form submission  

### 3️⃣ Server Setup and Testing
A local server was built to capture submitted credentials.  
Using `curl`, the data flow was tested to verify correct request handling.

### 4️⃣ DreamHost Deployment
To simulate a real-world attack:
- Registered a DreamHost domain  
- Uploaded phishing pages via FileZilla  
- Installed a free **Let’s Encrypt SSL** certificate  
- Tested HTTPS functionality  

### 5️⃣ Discord Bot Integration
An encrypted Discord webhook received submitted credentials, simulating exfiltration of stolen data in real time.

### 6️⃣ Awareness Landing Page
After users submitted their credentials, they were redirected to an **awareness page** explaining the phishing test and providing immediate security advice.

---

## 📊 Test Results
The phishing email was sent to **five employees**, producing the following results:

| Outcome | Description | Percentage |
|----------|--------------|-------------|
| ✅ Recognized the phishing attempt | Identified the email as fake and took no action | 20% |
| ⚠️ Clicked the link only | Clicked but did not submit credentials | 40% |
| ❌ Submitted credentials | Fell for the phishing attempt and entered credentials | 40% |

These results demonstrate that while some employees could identify the attack, additional awareness was necessary to reduce the risk.

---

## 🧩 Awareness Training
One week after the phishing simulation, a **phishing-awareness workshop** was delivered in collaboration with the Report team.  
Employees learned to:
- Verify sender domains and detect spoofing  
- Distinguish between HTTP and HTTPS websites  
- Inspect URLs safely before clicking  
- Recognize social engineering cues in emails  
- Report phishing attempts within the organization  

### 🧮 Analytics & Insights
With **Google Analytics**, we monitored:
- Click rates and engagement time  
- Navigation paths across the phishing pages  
- Credential submission behavior  

---

## 💡 Recommendations
1. Conduct recurring phishing-awareness training sessions  
2. Perform regular phishing simulations to reinforce vigilance  
3. Simplify the internal process for reporting suspicious emails  
4. Strengthen technical email filtering and warning mechanisms  
5. Enforce **multi-factor authentication (MFA)** for all accounts  

---

## 📸 Screenshots

### 📨 Example phishing email  
<img src="https://github.com/user-attachments/assets/96fee920-8d91-4e48-b8df-9ec257ebc31e" width="400"/>

### 🔐 Fake Report App login page  
<img src="https://github.com/user-attachments/assets/d58882b1-05e3-4b2e-a9f4-607270cd6efc" width="350"/>

### 📘 Awareness landing page  
<img src="https://github.com/user-attachments/assets/8c050ce1-ffc9-403d-9947-bde7abbb65c5" width="300"/>

### 🤖 Discord bot credential log  
<img src="https://github.com/user-attachments/assets/05577abf-99a6-48af-bd47-9a9b6e2997de" width="600"/>

### 📊 Google Analytics overview  
<img src="https://github.com/user-attachments/assets/ec37aa02-3e96-45a1-ae23-6fc9c0831d10" width="600"/>



---

### 🧾 Summary
This project demonstrates how controlled phishing simulations can effectively measure and improve an organization’s resilience to social engineering.  
It combined **offensive security techniques** (phishing design, credential capture) with **defensive education** (awareness training, analytics) bridging the gap between **attacker insight and user empowerment**.
