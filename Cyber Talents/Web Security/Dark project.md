# Challenge name: dark project

Link: https://cybertalents.com/challenges/web/dark-project

## Solution:
1) When you click on about in the navbar the url changes to: `darkp/index.php?home=about`

2) So, i though about the local file inclusion 
I used **Burp Suite** to try: 
  * `home=../../../../../../../../etc/passwd` 
  * `home=php://input&cmd=ls`
  
and both of them doesn't work 

3) Last thing: `php://filter/convert.base64-encode/resource=index`

![darkproject](https://user-images.githubusercontent.com/55226688/84811307-567c2600-b015-11ea-82a1-39ded654018f.png)

4) I used [DecodeBase64](https://www.base64decode.org/) to decode the code: 

![darkproject](https://user-images.githubusercontent.com/55226688/84811534-ad81fb00-b015-11ea-9a59-25d9e18d5af3.png)

