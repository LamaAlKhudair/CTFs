# Challenge name: catch me if you can

Link: https://cybertalents.com/challenges/web/catch-me-if-you-can

## Solution:
1) There wasn't anything helpful in the main page so I tried `/robots.txt` and it led me to those two pages 

![catchmeifyoucan](https://user-images.githubusercontent.com/55226688/84580076-4fb69e80-addc-11ea-85c5-f26336daec85.png)

2) When i opened `/source.php`. 

This code check if the password contains:`R_4r3@`, and match this format: `'/^-?[a-z0-9]+$/m'`

![catchmeifyoucan](https://user-images.githubusercontent.com/55226688/84580163-306c4100-addd-11ea-9271-7e542550fa46.png)

So I opend `/S3cr3t.php` and wrote `R_4r3@` as my password, the response was `ILLEGAL CHARACTERS`


3) So I used **Burp Suite** to edit the request, and tried this password: `123\nR_4r3@` 
and still the result was `ILLEGAL CHARACTERS`!

4) after many number of attempts I used the hex value for `\n` which is:`%0a`, so I tried this password: `123%0aR_4r3@`

![catchmeifyoucan](https://user-images.githubusercontent.com/55226688/84580406-55fa4a00-addf-11ea-9f73-581afa81ca2e.png)

so notice the end of the page there is this weird code. This code called BrainFuck and I used this great website to decode it [DecodeFR](https://www.dcode.fr/brainfuck-language)

![catchmeifyoucan](https://user-images.githubusercontent.com/55226688/84580579-c9e92200-ade0-11ea-9e0d-f80c4d72bf0a.png)

