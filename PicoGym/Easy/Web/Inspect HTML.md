## Challenge Name: Inspect HTML
Category: Web Exploitation, 
Solves: 108,509 

Challenge Description: 

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/inspecthtml3.png>)

## Method Walkthrough 
### Solving by Pico Browser Webshell

After starting your instance, you should've received a link to the challenge website!
Here's what you should see:

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/inspecthtml.png>)

Nothing appears to be useful. After some snooping around, it just seems like a page of plaintext. 

Let's use the hint and inspect the HTML. You can right-click and use 'Inspect', or type in "view-source:" ahead of the URL:


![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/inspecthtml2.png>)

Bingo! We've found the flag.

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/inspecthtml4.png>)

*Note: Make sure to only enter the given content of the flag wrapper: picoCTF{XXX}. The arrows around the flag in the image are not parts of the actual flag.

