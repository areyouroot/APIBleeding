# APIBleeding

this is a sample implementation of the API bleeding attack and a POC (proof of concept)

## Introduction

API Bleeding is an API injection attack that can be used to perform the SQL operation using the API

this type of attack can also leak the technology used.

this type of attack is always a combination of API injection with a path traversal attack or any other HTML header or request attack

sometimes even we can combine it with client-side attacks like XSS etc .....

### Breif on API attacks

there are many ways API attacks can be triggered.

1. API attack that performs read write operation without the authentication

2. injection of API in the request params 

3. MITM who modify the API calls

4. XSS or other injections that cause API injection

5. direct modification of the URL

## what is API Bleeding and How it Works

This is similar to an API injection attack but this is possible only once a custom API can be created and stored by the user that can be exploited in different ways you can create an API call that can elevate the privilege of a user or an API call that perform the crud operations etc.

eg: if you can create a GitHub page that triggers the GitHub API without triggering the page itself

![the API bleeding chart](apiBleedingChart.png)

### How bleeding API attack can damage your system

1. Path transversion attack + API injection.
    - Eg: the path can be redirected and all the files can be accessed

2. Database crud operations that can cause data leaks or damage.
    - similar to SQL injection and this also can execute critical commands like drop etc.

3. privilage esclation attack
    - if the API is triggered by admin or any high privilege user then they can give access to the other users.

4. Information disclosure.
    - some API call failures can leak some critical information like version or external DLLs etc.

5. XSS and other website related attacks.
    - OWASP top 10 can be performed etc .

# POC yet to be published using the angular website
# web attacks VM box yet to be published (CTF)