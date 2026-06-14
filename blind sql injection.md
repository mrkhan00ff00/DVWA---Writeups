# Blind SQL Injection: The Hidden Vulnerability

Description

Imagine you are trying to guess a secret password written on a piece of paper inside a locked box. You can’t open the box, and you can't
see the paper. However, you can ask a guard a single "Yes" or "No" question about what is written on it. If you ask, "Does the password 
start with the letter A?" and the guard nods yes, you just learned a piece of the secret. If you repeat this process over and over, you 
can eventually guess the entire password, one single letter at a time.

This is exactly how **Blind SQL Injection (Blind SQLi)** works. Unlike regular SQL injection—where the database explicitly errors out or
dumps secret data right onto the screen for you to see—a blind SQL injection gives the attacker absolutely no direct data on the webpage. The application's visual output stays exactly the same.

Instead, the attacker injects clever "True or False" statements into the input fields. By observing how the server responds, they can 
steal data. This usually happens in one of two ways:

* **Boolean-Based:** The attacker looks for subtle changes in the web page's behavior. For example, if a statement is true, the page
*  loads normally; if it is false, a small error message appears or a specific button disappears.
* **Time-Based:** If the webpage doesn't change at all, the attacker forces the database to pause or sleep for a few seconds if a
*  condition is true. If the page takes 5 seconds longer to load, the attacker knows their guess was correct.

Because it requires asking hundreds of yes-or-no questions to extract data, attackers rarely do this by hand; instead, they use
automated scripts to systematically rebuild entire databases character by character.

 What We Learned

* **Silence Isn't Security:** Just because an application doesn't show database errors or visible data leaks on the screen does not
*  mean it is safe from SQL injection.
* **Inference Attacks:** Attackers can reconstruct sensitive information entirely through side channels, such as observing conditional
*  page rendering (Boolean) or server response delays (Time-based).
* **Parameterized Queries are Mandatory:** The only definitive way to stop Blind SQLi is to treat all user input strictly as data, never
*  code, by implementing prepared statements and parameterized queries.



#CyberSecurity` `#WebSecurity` `#AppSec` `#SQLInjection` `#BlindSQLi` `#EthicalHacking` `#OWASPTop10`

###  Commands  ###

<img width="665" height="128" alt="Screenshot From 2026-06-14 11-12-34" src="https://github.com/user-attachments/assets/9f90f84a-7d35-4420-a0c4-024a173eb632" />
<img width="665" height="128" alt="Screenshot From 2026-06-14 11-12-46" src="https://github.com/user-attachments/assets/4c5bd3f3-3c7c-4cb2-80d1-b4e12355caf9" />

###  RESULTS  ##
<img width="666" height="267" alt="Screenshot From 2026-06-14 10-51-50" src="https://github.com/user-attachments/assets/a6b23a15-0344-4a92-8648-9b30033c282a" />
<img width="654" height="270" alt="Screenshot From 2026-06-14 11-19-43" src="https://github.com/user-attachments/assets/20f544d4-efeb-4ea2-ac21-19cdb971ea13" />
<img width="654" height="270" alt="Screenshot From 2026-06-14 11-19-56" src="https://github.com/user-attachments/assets/cbc2292b-beff-450b-9b28-d10b1a7a2d03" />
