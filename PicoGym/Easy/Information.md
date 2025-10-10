## Challenge Name: Information
Category: Forensics, 
Solves: 135,732

Challenge Description: 
![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-10%20193343.png?raw=true>)

## Method Walkthrough 
### Solving by Pico Browser Webshell

We are given a helpful hint telling us to look at the image details of cat.jpg

Firstly, we download cat.jpg into the Pico browser webshell. Copy the link address of the image file (by right-clicking on the hyperlink) and paste the link after the words 'wget'. 

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-10%20193430.png?raw=true>)

“Wget https://yourlink.net/yourimage.jpg”  ← The 'wget' command is a Linux command-line tool that you can use to download files. We use it in the webshell. 

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-10%20193458.png?raw=true>)

Cat.jpg should now be saved to your directory. You can access this file directly in the webshell. 

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-10%20193533.png?raw=true>)

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-10%20195307.png>) 

### Reflections



---
[Back to home](<https://github.com/eliu-civ/CIV-CTF-Writeups-/tree/main/PicoGym/Easy>)
