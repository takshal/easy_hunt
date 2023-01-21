# Rate limit Bug

## where to test(common place to test)?
1. password reset link
2. login page
3. change password function(old password confirmation)
4. comments


# steps to test
1. capture the password reset request in burp
2. send request to intruder
3. select any position 
4. go to payload select null payload(50)
5. click on attack
6. check if you got 50 password reset link on your email or not


# Rate limit bypass Techniques

# there are four way to bypass
1. customizing HTTP methods
2. adding header IP
3. adding null characture on email
4. using IP rotate Burp Extentions


## bypass rate limit using customiz HTTp methods

1. if request pass on GET then you can change it to POST,PUT,etc...
2. fot API you can use head method

## adding header IP

you can add below header in request to bypass rate-limit

1. X-Forwarded: 127.0.0.1
2. X-Forwarded-By: 127.0.0.1
3. X-Forwarded-For: 127.0.0.1
4. X-Forwarded-For-Original: 127.0.0.1
5. X-Forwarder-For: 127.0.0.1
6. X-Forward-For: 127.0.0.1
7. Forwarded-For: 127.0.0.1
8. Forwarded-For-Ip: 127.0.0.1
9. X-Custom-IP-Authorization: 127.0.0.1
10. X-Originating-IP: 127.0.0.1
11. X-Remote-IP: 127.0.0.1
12. X-Remote-Addr: 127.0.0.1

## adding null characture on email

1. you can also use %00 on the end of email to bypass rate-limit
2. adding slash(/) at end in api to bypass rate-limit on API for example: abc.com/api/v1/login to abc.com/api/v1/login/
3. some common characters : %0d , %2e , %09 , %20 , %0, %00, %0d%0a, %0a, %0C

## Using IP Rotate Burp Extension

1. Try changing the user-agent, the cookies... anything that could be able to identify you
2. If they are limiting to 10 tries per IP, every 10 tries change the IP inside the header.
  Change other headers
3. Burp Suite's Extension IP Rotate works well in many cases. Make sure you have Jython installed along.

4. Here You'll everything you need - https://github.com/PortSwigger/ip-rotate

 


