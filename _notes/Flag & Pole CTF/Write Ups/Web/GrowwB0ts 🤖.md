
```
Challenge Title:** Find your robot to get the flag

Flag format:** GCTF{}

Author: @_0xPb

Challenge URL: https://gr0wwb0ts.vercel.app

```

Here, in the description it's saying "**Find your robot to get the flag**"

The first thing that came to my mind is to check for the`robots.txt` file.

1. Start by visiting the given website: [gr0wwb0ts.vercel.app](https://gr0wwb0ts.vercel.app/)
2. Examine Robots.txt: In web security, the **robots.txt** file is used to instruct web crawlers which parts of a website should not be crawled or indexed. To access it, simply add /robots.txt to the URL. For example: https://gr0wwb0ts.vercel.app/robots.txt.
3. **Flag Discovery:** After examining the `robots.txt` file, you should find a line that might look like this:

```
User-agent: *
Disallow: /admin
Disallow: /login
Disallow: /signup
Disallow: /worg
Disallow: /flag.txt
Disallow: /wwrg
Disallow: /Growwbot
Disallow: /wworg
Disallow: /wworG

Get your flag here: 

47657420796f757220666c616720627920676f696e6720746f20746865202f666c61672e747874

```

4. This instructs web robots not to access the `/admin, /login, 'signup, /worg, /flag.txt, /wwrg, /Growwbot, /wworg, /wworG'` file. However, for this CTF challenge, we are interested in finding the flag that's in the format of `GCTF{}`. 
5. Here the ASCII HEX data is present to confuse the players about the flag location `47657420796f757220666c616720627920676f696e6720746f20746865202f666c61672e747874`
6. You can access the endpoints directly by visiting: `https://gr0wwb0ts.vercel.app/wworg`
7. After accessing all the endpoints and checking for the flag. In one of the endpoints `/wworg`  I found another encoded string which I figured out as base64.
8. By visiting an online [base64 decoder](https://www.base64decode.org/)  and decoding the string. 
9. I got the flag `GCTF{y0u_mus7_r3m3b3r_th3_r0b0ts}`

## Flag:

`GCTF{y0u_mus7_r3m3b3r_th3_r0b0ts}`

Congratulations! You've successfully completed the "GrowwB0ts 🤖" challenge and obtained the flag hidden within the `robots.txt` file. This challenge tests your ability to identify and access hidden resources on a website.