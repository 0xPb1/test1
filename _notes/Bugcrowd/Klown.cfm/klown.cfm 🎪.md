---
Title: klown.cfm 🎪
Author: 0xPb
Date: 29th Oct, 2023
Categories: [CTF, spooky Challenge]
Tags: [bugcrowd, spooky, klown]
---

```
challenge URL: https://spooky.bugcrowd.zw.ink/klown.cfm
```

### Introduction

In this CTF challenge, you were presented with a mysterious web page at the given URL. The initial page seemed to have an inaccessible submit button, but with a little investigation, you were able to uncover a secret password. By following a series of steps, you successfully bypassed the security mechanism and retrieved the `CODE`. Let's walk through the solution:

## Solution:

1. **Initial Exploration:** 
	* Upon visiting the URL [https://spooky.bugcrowd.zw.ink/klown.cfm](https://spooky.bugcrowd.zw.ink/klown.cfm), I encountered a peculiar webpage.

![#1](https://raw.githubusercontent.com/0xPb1/test1/main/_notes/Bugcrowd/Klown.cfm/Pasted%20image%2020231101223651.png)

2. **Hidden Button Element:**
	* I noticed a button element with the following attributes:

```
<input name="smile" type="submit" value="submit" disabled="true" style="color:#DF6322; font-weight:bold; cursor: not-allowed" title="Access Denied" id="smile">
```

* The button was initially disabled and appeared inaccessible.
	
3. **Button Activation:** 
	* I realized that the button could be activated by removing the disabled="true" attribute.
4. **Form Submission:**
	*  After removing the disabled="true" attribute, I submitted the form with the default input "Kreepy Klown denies you access!".
5. **Alert Popup:**
	* My action triggered a pop-up message that revealed the password:
		`Secret Password: KR33PIE-KL0WN`

![#2](https://raw.githubusercontent.com/0xPb1/test1/main/_notes/Bugcrowd/Klown.cfm/Pasted%20image%2020231101223939.png)

6. **Input Password:**
	* You then input the secret password, `KR33PIE-KL0WN`, into the appropriate field, following the instructions provided in the pop-up.
	
	![#3](https://raw.githubusercontent.com/0xPb1/test1/main/_notes/Bugcrowd/Pasted%20image%2020231101224233.png)

7. **Final Flag:** 
	- After submitting the password, you received the final response:

![#4](https://raw.githubusercontent.com/0xPb1/test1/main/_notes/Bugcrowd/Klown.cfm/Pasted%20image%2020231101224121.png)




Here's a link to the next fun [[Bugcrowd eLFI Challenge]].