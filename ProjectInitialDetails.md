Project Initial Details Submission 

 

Problem Statement and Target Users 

 

What real-world problem does your application aim to solve? 

 

Background information: 

With the rise of technology, scam emails like phishing attempts, fake job offers, and impersonation emails are becoming more legitimate and common. This may negatively impact schools as most schools use email as their primary communication channel; thus, students may get tricked into clicking on malicious links, revealing their personal information, or making illicit payments.  

This issue is prevalent and reflected in the recent news of at least 20 students who received emails from impersonators requesting urgent payment of school fees1. As a result, the victims lost over $30k to the scammers. 

 

Our goal: 

Given this, our goal is to create an application that helps students identify potential scam emails before they do anything. Our application analyses email and flags suspicious indicators, then subsequently provides a risk assessment and recommends the course of action the student should take. 

 

Who are the intended users of the application? 

The intended users are students who depend on email as their primary communication channel. Our application is designed to assist students in making more informed decisions when dealing with suspicious emails. 

 

 

User Inputs 

 

What information or data will users provide to the system? 

The users of the application will provide the system with input data such as the sender’s email address to verify if it is from a valid domain and the body content of the email that they have received to check for email content, attachments and links, to identify whether the email they received is a potential scam. 

 

 

Use of AI 

 

How will AI be utilized within the application? 

AI will be used to analyze the input from the user to determine the intent of the email, classify potential scam types (if applicable), analyze the language used to identify potential social engineering techniques, analyze the links and attachments in the body content to provide a risk score, and recommend the next course of action the user should take. 

 

What outputs, insights, or recommendations will the AI generate from the user inputs? 

The AI will analyze the user inputs and generate an output in JSON format containing information such as risk score, intent, scam type, social engineering techniques (if applicable), suspicious links (if applicable) and recommended actions before passing it onto the business logic layer. 

 

Business Rules 

 

What business rules, validations, or decision-making logic will be applied to the AI-generated outputs? 

After receiving the AI output in JSON format this layer will validate it in the correct data format and contain all the information required from the AI layer such as risk score, intent, scam type, social engineering techniques, suspicious links and recommended actions. Afterwards, there will be a multi condition decision rule combining the different data in the AI output to come to a decision. For example, if a risk score above 90 and suspicious link(s) count is more than 0 then the recommendation from the AI will be overwritten to “Block and Report” and we will rank the priority as critical.  

 

Repository Information 

URL of Repository: https://github.com/INF1103Team7/INF1103-Ai-Powered-Scam-Message-Risk-Detector

 

References 

1 Chia, L. (2026) ‘Students lose over $30k to scammers impersonating educational institutions’, The Straits Times, 19 March. Available at: https://www.straitstimes.com/singapore/at-least-31000-lost-to-scams-involving-impersonation-of-educational-institutions-in-under-3-weeks (Accessed: 16 September 2026). 