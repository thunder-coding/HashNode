## How to make your Web Servers more secure

Everyday, we hear a news that the server of X company was hacked. Some rich peoples' social accounts where hacked. 


![photo-1526374965328-7f61d4dc18c5.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1603421499272/LupmiD5fJ.jpeg)

## Have you ever wondered, why such things happen?

These all cyber attacks happen only because of vulnerabilities in the server. Vulnerabilities, in the sense data exposed which was not supposed to be.


<br>
## About Me:

Hey there 👋👋, I am Yaksh Bariya, a 14-year coder who is very much interested in technology. Today, in this article I am gonna give you a lot of valuable resources and information about how can you make your server more secure.


## Why is cybersecurity becoming a hot 🔥 topic?

Everyday about 30,000 new websites are hacked 🔓 daily. That's a huge number. Most of these websites are commercial sites of small business companies.


## If hackers are trying to hack servers and developers know about this, why don't they make their sites secure?

Well they do, but hackers now-a-days are smart enough to penetrate into a highly secure server without much difficulties


## What can hackers do with your data?

They can do a lot. They can sell all your server data on Dark Web 🕸️. They may also ask you for a ransom in the form of cryptocurrency (BitCoin or something).


## How hackers hack?

Before diving into deep & advanced Cybersecurity, let's understand how hackers steal your protected secret and confidential data.

Understand hacker like a thief who wants to steal your money & gold. I suppose you are smart enough to get that our money and gold is the server data hackers want to steal 😉.

Now, say you have to go somewhere out of your home 🏠 due to some work and the thief rolls into your house for stealing all your stuff. This is the period when hackers are trying to attack into your system. Note: the thief may also come when you are home.

Now, if we as a smart person like the kid in the **Home Alone**(I hope you all have seen this movie) then the thief will never ever think even to hack again any small server.

If you aren't, then the thieves will easily steal all your wealth 🤑.


### Let's come back to the topic

## How can you make your server more secure 🔐  ?

Well there are many ways to do that. Each way implemented means security level increases by some factor.


### 1. Rate limiting 

Rate limiting not only helps to prevent unnecessary traffic 🚦 on your server but can also prevent leaks of certain data from your server.

Many popular APIs have rate-limiting including GitHub API.

Well, You can increase the rate limiting limit for authenticated users like as in GitHub API.



### 2. Log everything

Logging everything may help you find any traces of previous attacks on your server and fix bugs in your server-side code so that such attacks can be minimised.


### 3. Never provide a direct access to any file on your server.

Direct access in the sense that anyone visiting your website should not be able to view the folder/file structure of your server.

You may be currently thinking what can the hacker do with your folder structure. Well he/she can do a lot. The hacker can get where all the databases are stored.


### 4. Check if all your database are encrypted and there is no way in there

Never expose your database. Always check if all your databases are not accessible to the general public before uploading your code to the server.

Encrypting databases is as important. Remember encryption will ensure that even after stealing your data the hacker is not able to access all the data


### 5. Minimise your server's dependency on third party services

Well third party services help a lot in decreasing load on our main server, but there are some issues with them as well.

#### Why minimise third party dependencies?

Third party companies can leak your data. Therefore, we should never completely rely on them.
Also most of the WordPress website leaks/hacks happen only because of third party plugins.


#### If you are using Node.js for backend developement 

- Make sure you are using packages that are being regularly updated and maintained. You can check if they are really maintaining the package by looking at their GitHub repository (look at the last commit date)
- Make sure you check their GitHub issues page to find any vulnerability


### 6. Make sure you don't expose your `.git` folder

Majority of developers are familiar with Git. Git is a version control tool.

If you are exposing your `.git` folders then you are exposing the whole source code of the site to attackers.



## Conclusion

These are just some important points which are very necessary. There are much more points. I would like to hear them in comments 👇.



### Sources:

- https://www.webarxsecurity.com/website-hacking-statistics-2018-february/

- https://www-zdnet-com.cdn.ampproject.org/v/s/www.zdnet.com/google-amp/article/new-gitjacker-tool-lets-you-find-git-folders-exposed-online/?amp_js_v=a6&amp_gsa=1&usqp=mq331AQFKAGwASA%3D