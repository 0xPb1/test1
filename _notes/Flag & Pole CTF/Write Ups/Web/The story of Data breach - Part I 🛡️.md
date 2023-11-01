
```
One of the Microsoft's employee requested for the help from Groww's security team to deploy the [shield portal](https://shield.growwinfra.in/) in microsoft's infra. But unfortunately he/she exposed the login credentials by mistake, but don't know where exactly.

Please help him find the exposed credentials.

Flag format: GCTF{username:password}

Author: @rohitcoder
```

### Introduction 

This challenge is set in a scenario where a Microsoft employee accidentally exposed their login credentials on the "shield portal." Your task is to find these exposed credentials within the JavaScript files and follow the flag format.

## Solution:

1. **Initial Visit:** Start by visiting the "shield portal" at [shield.growwinfra.in](https://shield.growwinfra.in/).
    
2.  **Inspect JavaScript Files:** Right-click on the webpage and select "Inspect" or use the browser's developer tools to examine the source code, especially the JavaScript files.
	
3. **Locate and Open JavaScript File:** The challenge provides you with a specific JavaScript file to investigate: [connect.js](https://shield.growwinfra.in/static/external/connect.js). This file is where the exposed credentials are hidden.
    
4. **Flag Discovery:** Your mission is to find the username and password within the JavaScript code. Search for comments or variables that might contain these credentials.
    
5. **Extract the Flag:** When you discover the exposed username and password, note them down in the correct flag format: `GCTF{4dm1n:nWaWlpkC8cArTLUM}`.

## Flag:

`GCTF{4dm1n:nWaWlpkC8cArTLUM}`

Congratulations! You've successfully completed the "**The story of Data breach - Part I 🛡️**" challenge by locating and extracting the exposed login credentials from the provided JavaScript file on the shield portal. This challenge tests your JavaScript code examination skills and your ability to identify security vulnerabilities.