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

### The 'License' description of the image contains a suspicious sequence! 

### If you are unfamiliar with cryptography (if you are familiar skip down to the next section):

Use this website: https://www.dcode.fr/cipher-identifier 
Paste the suspicious sequence into it and it will tell you the most likely encryption on the left. 
It will then direct you to the appropriate decrypter. 

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-13%20105337.png>)

### Use the base64 decrypter (image on the right) to find the flag! 

### If you have some cryptography experience:
You'll likely recognize that this is a base64 sequence. 
You can directly decipher the sequence in your webshell using the following command:
    echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | base64 -d

## All in all, you should finish with the correct flag picoCTF{the_m3tadata_1s_modified}!
### Congrats! You just found a flag! Submit it into the challenge. 

### Similar PicoGym Questions
This is a classic Forensics challenge combining elements of ciphers and image analysis. If you enjoyed this question check out:
- hashcrack (Easy, picoGym)

---
[Back to home](<https://github.com/eliu-civ/CIV-CTF-Writeups-/tree/main/PicoGym/Easy>)
