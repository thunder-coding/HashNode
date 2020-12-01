## Code Obfuscation : Why, How & When...

With huge number of available code decompilers out there on the internet, it is becoming more important day by day to hide our source code, so that any reverse engineer cannot decompile it.

Interpreted languages like Python & JavaScript have made obfuscation more necessary to protect the source code. Even though you package your app as an executable, you source code can still be viewed from the memory.




# What is Code Obfuscation?

Code Obfuscation is the technology for making lives of reverse engineers hard so as to keep our source code safe.

It's similiar to the Oxford provided defination for **obfuscation** *`the action of making something obscure, unclear, or unintelligible.`*

Code Obfuscation is the process of converting the actual source code to a unreadable and un-understandable code.

## Here's a Javascript Obfuscated Code Example

- Real Source Code

```javascript
function hi(){
    hi();
}
hi();
```
- Obfuscated Code

```javascript
var _0xcd38=['log','Hello\x20World!'];(function(_0x1499a2,_0x273593){var _0xcd38c1=function(_0x13863e){while(--_0x13863e){_0x1499a2['push'](_0x1499a2['shift']());}};_0xcd38c1(++_0x273593);}(_0xcd38,0xd7));var _0x1386=function(_0x1499a2,_0x273593){_0x1499a2=_0x1499a2-0x1a2;var _0xcd38c1=_0xcd38[_0x1499a2];return _0xcd38c1;};function _0x425006(){var _0x18303c=_0x1386;console[_0x18303c(0x1a3)](_0x18303c(0x1a2));}_0x425006();
```


# How does Code Obfuscation work?

As you can see, in the obfuscated code, the variable names have been changed, function name changed into random hex.

Also, unnecessary variables and loops have been added so that no reverse engineer can understand it.


I would also recommend you to experiment with it yourself, [here is the link to the online JavaScript obfuscator which I used in the above example](https://obfuscator.io/)


# How is Code Obfuscation different from Code Uglifying

Code Uglifying is very different from Code Obfuscation. Code Uglification only removes excess space characters and tab characters, the uglified code can be easily brought back to it's earlier state using Beautifier use as Prettier for VS Code.



# Why obfuscate your code?

Let's say you and your team is working hard on a new commercial application for your company. The application is obviously paid 💰. You released the first public version (v1.0.0).

Now, after 2 days you get to know that your app is available as a free download on a 3rd party torrent website. You would be too sad after hearing this news.

Your months and years of hard work was stolen!!

## This situation could be prevented.

### How?

If you had obfuscated your Source Code before compiling it and releasing.

### How can Obfuscation prevent that? 😏

Obfuscation will prevent your application's real source code from being viewed by any reverse engineer.

### But how?

As mentioned earlier, code Obfuscation changes variable names, line numbers, adds unnecessary loops so that it would become hard to understand it.


# How to obfuscate your code?

There are many obfuscaters available on the internet, most of them are free and Open Source.

To obfuscate your code, first of all you need to install an obfuscater. Then just follow their documentation 😉.

## Here is a list of different obfuscators for different languages:

- Java

### [ProGaurd](https://www.guardsquare.com/en/products/proguard)

Certainly the most popular and widely used Java Obfuscater.
Comes pre-installed with Android Studio.

[See a more bigger list of Java Obfuscaters here](https://java-source.net/open-source/obfuscators)


- JavaScript

### [javascript-obfuscator](https://obfuscator.io/)

Open Source JavaScript obfuscater. 

Available as a npm package 📦 

```
$ npm install --save-dev javascript-obfuscator
$ # OR
$ yarn add --dev javascript-obfuscator
```

- Python

### [PyArmour](https://pypi.org/project/pyarmor/)

Install
```
$ pip install pyarmor
```

- [C#](https://github.com/obfuscar/obfuscar)

An Open Source C# obfuscater for you


- [Android Studio](https://developer.android.com/studio/build/shrink-code)

Android Studio's official guide to obfuscate your app.


- C/C++

C or C++ does not require obfuscation. As C++ is directly compiled to machine language, decompiling it will give us only Assembly, which is very hard to understand


# How safe Code Obfuscation is?

Code Obfuscation is safe. But still I would recommend you to first test your app compiled with obfuscated code before releasing it.

Also, while testing before production should be done without obfuscation, as obfuscation is very time consuming many times.


> Also remember

Your obfuscated code will be safer, but not safest.


# Advantages and disadvantages of Code Obfuscation

## Advantages

Code Obfuscation has many advantages

- Code Shrinking

Code Obfuscation often removes unused code.

For example, if your code has a if statement with a empty `else{}`, then the else will be removed during obfuscation

- Source Code protection

It's too obvious 😜

- Optimisation

As a result of Code Shrinking, the obfuscated code is often more optimised



## Disadvantages

Well, there are a huge number of advantages, there are also much more disadvantages too.

- Malicious applications are often obfuscated

Many of the malicious app creaters obfuscate their code so as to bypass Antivirus protection.

- Antivirus often goes mad

Whenever you visit a website which has obfuscated code, sometimes your antivirus becomes mad. This is because, many sites obfuscate their code to hide malicious 


- Obfuscated Browser Extensions no longer on Chrome & Firefox

As Obfuscation is often used to hide malicious code, this action was announced by Google and Mozilla.

> Fact: 70% of extensions removed from the Chrome Web Store were obfuscated.


- Many a times obfuscation is time consuming

I would always recommend you to test your app or anything without obfuscation first, then again test it after obfuscation.





# Summary

Code Obfuscation is very important of you are working on a huge app.

There are a lot of decompilers available on the internet.

Code Obfuscation can protect your code to a huge extent, but remember that everything is hackable.


## Reply in comments 👇
## Do you obfuscate your code?


 
## Still here?

I have something special for you...

Follow me on [Twitter(@CodingThunder)](https://twitter.com/CodingThunder) to see my #100daysofcode progress. I also share some good threads sometimes. :)

Have a nice day..