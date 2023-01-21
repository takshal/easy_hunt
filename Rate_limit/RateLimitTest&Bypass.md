# Rate limit Bug

# where to test(common place to test)?
1. password reset link
2. login page
3. change password function(old password confirmation)
4. comments


# steps to test
1. capture the password reset request in burp
2. send request to intruder
3. select any position 
4. go to payload select null payload(50)
5. click on aytack
6. check if you got 50 password reset link on your email or not


# Rate limit bypass Techniques

# there are  way to bypass
1. customizing HTTP methods
2. adding header IP
3. adding null characture on email
4. using IP rotate Burp Extentions
 

