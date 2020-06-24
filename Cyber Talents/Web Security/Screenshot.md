# Challenge name: Screenshot

Link: https://cybertalents.com/challenges/web/screenshot

## Solution:
 
 1) We'll try LFI so add this to the link `?url=&server=php://filter/convert.base64-encode/resource=internalapi4.local/../index.php`

2) Open this image in new tab and download it as `jpg`

![screen](https://user-images.githubusercontent.com/55226688/85483252-244a6580-b5cd-11ea-8014-f4e552e79f76.png)

3) Open it with Notepad 

![screen](https://user-images.githubusercontent.com/55226688/85483545-af2b6000-b5cd-11ea-91fd-c55552ce7018.png)

4) Decode it with [Base64](https://www.base64decode.org/)

