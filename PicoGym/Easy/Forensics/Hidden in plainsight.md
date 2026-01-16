🐣 You just found a special flag!
If you're reading this outside of club hours after our 'information' demo, show Emma civ{b3tt3r_7h4n_7h3_r35t} for a special treat next meeting! :)

## Challenge Name: Information
Category: Forensics, 
Solves: 2,669

Challenge Description: 
![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-22%20161300.png>)

## Method Walkthrough 
### Solving by Pico Browser Webshell

We'll just continue off of in-club progress! 

After decrypting the base64 sequence from the image meta, you should've gotten this:

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-22%20162140.png>)

We are given legible text saying 'Steghide'. You should've done research on this in-club and discovered that this is a steganography program that hides data in things like images! 

Now, in CTFs, TRY EVERYTHING THAT'S SUSPICIOUS! 
Usually, an equal sign is a key suspicious indicator of a cipher! Let's decrypt the second sequence given after the colon:

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-22%20162544.png>)

Bingo! Looks like we got something legible. It's not quite the flag yet because flags are usually written in leet speak, but what we know now is that this image was hidden using steghide and the passphrase is 'pAzzword'!

The best way to go from here is to directly use webshell commands. 
You should've downloaded img.jpg, so run the following to extract the flag with '-p' to give the passphrase we found:
steghide extract -sf img.jpg -p pAzzword

Bingo! We've been given the flag in a .txt file!

You can view the file using 'nano filename' or 'cat filename'. 

![img](<https://github.com/eliu-civ/CIV-CTF-Writeups-/blob/main/PicoGym/Easy/Images/Screenshot%202025-10-22%20163713.png>)

Congrats! You just found the flag! 

If you found this challenge interesting, try CanYouSee!









