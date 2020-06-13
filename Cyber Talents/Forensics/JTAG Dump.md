# Challenge name: JTAG Dump

Link: https://cybertalents.com/challenges/forensics/jtag-dump

## Solution:
1) Run `file` command

![jtag](https://user-images.githubusercontent.com/55226688/84557155-5b00c000-ad31-11ea-81ef-e341176e0d08.png)

2) Use `binwalk` to extract the files

![jtag](https://user-images.githubusercontent.com/55226688/84557260-28a39280-ad32-11ea-8024-ff86e175b584.png)

3) You'll find the flag in one of the images: `9ABFF`
