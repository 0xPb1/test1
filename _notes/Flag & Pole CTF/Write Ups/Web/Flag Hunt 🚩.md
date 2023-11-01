
```
There is some interesting information hidden around this site. Can you find it?

Flag format: GCTF{}

Author: @_0xPb

[flag-hunt-alpha.vercel.app](https://flag-hunt-alpha.vercel.app/)
```

This challenge is a simple scavenger hunt challenge for flags. It presents a web scenario where you need to explore a website and find hidden flags in various locations. Your mission is to uncover the flags and extract them.

### Flag 1: In the Source Code
1. **Initial Visit:** Start by visiting the website: [flag-hunt-alpha.vercel.app](https://flag-hunt-alpha.vercel.app/).
    
2. **View Page Source:** Right-click on the webpage and select "View Page Source" or use the browser's developer tools to inspect the source code.
    
3. **Flag Discovery:** Search through the source code for any comments, hidden HTML elements, or JavaScript code that may contain the first flag. It should be in the format `GCTF{d3v's_`.

### Flag 2: In the CSS File

1. **Explore CSS Files:** Continue to explore the source code, focusing on the CSS files used by the website. These files are typically linked in the HTML source.
    
2. **Flag Discovery:** Search through the CSS files for comments or hidden CSS classes that may contain the second flag. It should also be in the format `can_be_`.

### ### Flag 3: In the `robots.txt` File

1. **Examine Robots.txt:** Just as in the previous challenge, check the `robots.txt` file. To access it, add `/robots.txt` to the URL, e.g., `https://flag-hunt-alpha.vercel.app/robots.txt`.
    
2. **Flag Location:** Look for any disallow rules that specify files or directories that web robots should not access. One of the disallowed paths might point to a file that contains the third flag.
    
3. **Access the File:** Once you've identified the disallowed file, visit it directly by appending it to the website's URL. For example: `https://flag-hunt-alpha.vercel.app/flag1.html`.
    
4. **Flag Extraction:** Open the disallowed file to discover the flag. It should be in the format `cool_h4ck3rs}`.

## Flags:

 `GCTF{d3v's_can_be_cool_h4ck3rs}`

Congratulations! You've successfully completed the "Flag Hunt 🚩" challenge by uncovering the hidden flags in the source code, a CSS file, and a file referenced in the `robots.txt` file. This challenge tested your web enumeration and investigation skills, making you a web flag-hunting expert!