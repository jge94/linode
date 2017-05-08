# Linode Registration Instructions

1. Go to link [https://manager.linode.com](https://manager.linode.com/)
2. Click Sign up and create an account
3. Click on "OK! Let's complete my sign up"
4. Enter your information: choose pre-load $5, enter a credit card, but this will be a free trial (you can cancel it within 7 days)
5. When submitted, copy the IP address line: "root@YOUR_IP_ADDRESS"
6. Go to terminal, and do "ssh" then copy the IP address line <br/>
For example, <code>ssh root@97.107.142.240@</code>
7. For "Are you sure you want to continue connecting (yes/no)?", enter yes
8. Enter your password
9. vi /etc/ssh/sshd_config
10. ??? turn off root
11. Enter: <code>adduser YOUR_USER_NAME</code>
12. Enter your password, and retype
13. You can leave all the rest of the information to be blank, keep hitting enter
```
Full Name []: 
Room Number []: 
Work Phone []: 
Home Phone []: 
Is the information correct? [Y/n]
```
14. <code>su YOUR_USERNAME</code>
15. <code>sudo apt-get update</code>
16. <code>su root</code>
17. Enter password
18. <code>usermod -aG sudo YOUR_USERNAME</code>
19. <code>su YOUR_USERNAME</code>
17. Enter password
20. <code>sudo apt-get update</code>
21. <code>sudo apt-get install nginx</code>
Done


