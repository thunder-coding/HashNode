## Why should you learn TypeScript

## Today's quote

>I AM NOT DISCOURAGED BECAUSE EVERY WRONG ATTEMPT DISCARDED IS A STEP FORWARD

 ~ Thomas Edison
![](https://lh3.googleusercontent.com/proxy/96l8CUusLGBk3NUA9Gf-uf63bpsVnxfmriZjdeqHinD5wghix85Fkj2b-GTkjQQsyg5WvVAZSC5TJYyTnOAhPkf7NG3Tn5_P7GZ8HFFXS95XObfsynhJhQ9za9L4Jj0ZDBvOEg5EDZb5MARBKwTVMIgWj5TWZ1751FM9CY5Bzxq8adeD5rkPkCHCL74IutXDlrNaID8URtJ0GvO-nqLkbg=w430-h342)


## Some facts about TypeScript

- TypeScript was developed by **Microsoft** about 8 years ago (first public release: 1 October 2012)
- **TypeScript** is a superset of **JavaScript**, which means that every valid JavaScript code is a valid TypeScript code
- TypeScript is written in TypeScript. That's called recursion
- Morever, TypeScript source code is available on [**GitHub**](https://github.com/microsoft/typescript) with 8.7k+ forks and 65.2k+ stars ⭐ 
- TypeScript is compiled to JavaScript
- C# and TypeScript were developed by the same developer, **Anders Hejlsberg**

<br>

Now let's talk about the real stuff. 
# Why should you learn TypeScript?🤔

## 1. TypeScript provides you with types in JavaScript.

### What does that mean?

JavaScript not provide you to define the type of variable you want while declaring it. The type keeps changing according to the value assigned to it.

But using TypeScript you have this feature

TS
```
var hello:String = "Hello World";
```
JS
```
var hello = "Hello World";
```


TypeScript Compiler compiles your `*.ts` file and checks for any errors in types. If you try to assign another type of value to a variable, then your **TypeScript Compiler** will surely give you an **error**.

Means if you write this code
```
var hello:String = "Hello World";
hello = 123;
```

Then you will get this error `Type 'number' is not assignable to 'String'`

Looks like a nice catch, isn't it

Im different words TypeScript is strongly typed language

![](https://media1.tenor.com/images/c2e93fddc36fb0ef68d5d843ced23f1b/tenor.gif?itemid=15242113)


## 2. TypeScript is Open Source

What makes a developer feel more proud then using an **Open Source** software? Nothing, Yeah!😇

![](https://media3.giphy.com/media/HvvpNczg8Dcw8/giphy.gif)


## 3. Huge community

TypeScript has a huge community of developers on **Stackoverflow** and other sites. So, if you will ever fall in some problem, there will be always someone to help you out.


## 4. Better for huge projects

**TypeScript** is mainly used for large projects becuase it provides much better exception catches.

Some awesome examples of Open Sourced TypeScript projects:

<ul>
    <li>[Visual Studio Code](https://code.visualstudio.com)</li>
    <li>[Google's Open Source UI framework Angular](https://angular.io)</li>
    <li>[Tensorflow](https://Tensorflow.org)</li>
    <li>[And even GitHub Desktop](https://desktop.github.com)</li>
    <li>[Vue JS](https://vuejs.org)</li>
</ul>


## 5. Much more like other popular languages like C#, C++, or Java

Many people feel that TypeScript is much related to C# because TypeScript's syntax is much more similar.

### A default support for enum

Yeah! You heard that right. TypeScript has a default support for enum classes which is very much similiar to that of C++.

```
enum S {
    NO = 0,
    YES = 1
}
```

### Unions in TypeScript

If you have learnt C or C++, then you may be probably familiar with `union` types.

Unions in TypeScript are somewhat different from them. In TypeScript `union` is a variable with multiple types.

Example of union in TypeScript
```
let myVar : string | number;        //Variable with union type declaration
 
myVar = 100;            //OK
myVar = 'Lokesh';       //OK
 
myVar = true;           //Error - boolean not allowed
```



<br>
<br>






![ts-logo-512.svg](https://gist.githubusercontent.com/thunder-coding/39b754acc2878718f198eebabe9bba49/raw/946d404189a1b1de8ec8cd2aa99fdd64c870535e/TypeScript-Logo.svg)

# TypeScript Tutorial



## We currently read why should you learn TypeScript , now let us code some TypeScript

Before you start with this tutorial make sure you know some basics of
- JavaScript
- HTML
- CSS

## Installing TypeScript

Before running and/or compiling TypeScript you need to install the TypeScript Compiler first. You have mainly 3 ways to use TypeScript

### Installing TypeScript package 📦 using npm

![nodejs logo](https://nodejs.org/static/images/logos/nodejs-new-pantone-white.svg)

- First download and install node.js from https://nodejs.org
- Open a fresh new terminal and run `node -v`.
If you get something like `v14.14.0`, congrats your installation is successful
- After the installation is successful run `npm install -g typescript`
- Check your TypeScript installation by running `tsc -v`


### Using TypeScript from your browser

Just open [TypeScript Playground on your browser](https://www.typescriptlang.org/play)

[![Screenshot of typescriptlang.org/playground](https://www.typescriptlang.org/static/play-fa691fca179c9ba4e0d764bd0e67c5aa.png)](https://www.typescriptlang.org/play)


### Installing plug-in/extension directly in your IDE

Search for TypeScript Compiler in your IDE, check if you get one, if not follow any above method. If you are using Visual Studio IDE, then you should get the TypeScript extension on [Marketplace](https://marketplace.visualstudio.com/items?itemName=TypeScriptTeam.typescript-403)

## Coding our TypeScript file

I strongly recommend you to use a Code Editor during this tutorial, it will give you syntax highlighting, which will help you a lot. Incase you don't have one get any one of these

- [VS Code](https://code.visualstudio.com)
- [Notepad++](https://notepad-plus-plus.org/downloads/)
- [Sublime Text 3](https://www.sublimetext.com/3)




### Let's create a new TS file

Create a new blank folder, and open your code editor there. In your editor create a new file with any name you want and at the end `.ts`. This `.ts` file is your TypeScript source file.

I gave the name `index.html`.


### Let's write some code

Open your TypeScript file. And type the following code
```
const date:Date = new Date();
const hour:Number = date.getHours();
const minute:Number = date.getMinutes();
const seconds:Number = date.getSeconds();
console.log(`The time is ${hour} : ${minute} : ${seconds}`)
```

This simple TypeScript program will give you the current time.

### Compiling TypeScript

Browsers and other JavaScript engines can't run TypeScript, you need to compile it first.

Let's compile it.

Open your terminal in the Current Directory.

> Quick Bonus Tip:
If you are using VS Code, you can open terminal directly by dragging from the top of the bottom status bar.

To compile your TypeScript file run `tsc <filename>` in your terminal. After the compilation, you should get the `*.js` file in the same directory with the same name.

If you get any errors while compiling TypeScript, make sure you did it correctly.


### Running the compiled JavaScript.

You can run your compiled JavaScript in either your browser console or node.js

To run in node.js

Run `node <filename.js>` in your terminal.
Hurray!! You learnt some basics of TypeScript.




<br>
<br>
<br>

Some recommended YouTube videos you must watch


%[https://www.youtube.com/watch?v=BwuLxPH8IDs]


<br>
<br>

Now, if you have read this far consider following me on [Twitter(@CodingThunder)](https://twitter.com/CodingThunder)

If you liked this article, don't forget to like❤️, share and drop your valuable suggestions in the comments section below.