# Introduction 

## Welcome to the Basic [Express][express] App guide :rocket:

[Express.js][express] is a fast, minimalist web framework for [**Node.js**][node], making it easy to build powerful and scalable web applications. Whether you're new to backend development or just getting started with Express, this guide will walk you through the fundamentals of setting up a basic Express app!

> [**Node.js**][node] (or informally Node) is an open-source, cross-platform runtime environment that allows developers to run JavaScript on the server. Node provides an environment to run scripts server-side to produce dynamic web content for the client.

> [**JavaScript**][js] is a programming language used to make web pages interactive. It runs in the browser and on the server (with Node.js), allowing developers to create dynamic websites and applications.

## Prerequisite readings:
1. **Very basic** CLI (Command Line Interface) understanding.
> Basically, knowing where the CLI is located and being able to access it.
2. **Some** [_Node.js_][node] knowledge.
> The commands will be given, but it is very much recomended to understand why they are being used.
3. **Basic** [_JavaScript_][js] knowledge
> The commands will be given, but it is very much recomended to understand why they are being used.
4. **Basic** [_HTML_][html] knowledge
> The text will be given, but it is very much recomended to understand why it is being used.
5. **Some** [_GitHub_][git] understanding.
> Understanding how to create a repository. This will only be needed for hosting and a [guide][gitGuide] will be attached.

## What You'll Learn :book:
- How to install and set up Express
- Creating a basic web server
- Handling simple routes (GET, POST)
- Handling different content types in Express
- Error handling in Express
- Running the app in a browser
- [Hosting](Glossary.md) your app

## Why use Express
- Much simpler than alternatives
- Nicely integrated with [JavaScript][js]
- Supports hundreds of packages
- Vast documentation

## Intended users
This guide is designed for **beginners** who want to learn how to set up and use **Express.js** to build a simple web server. It is ideal for:

* **New Developers** - Those who are just starting with backend development and want an easy-to-follow introduction to Express.
* **JavaScript Learners** - Developers familiar with JavaScript who want to explore how it works on the server-side.
* **Frontend Developers** - Those who know HTML, CSS, and JavaScript but want to expand their skill into backend development.
* **Students & Hobbyists** - Anyone curious about how to create simple [_APIs_][api] and web applications using Express.js

> [**API(Application Programming Interface)**][api] is a way for different applications to communicate with each other. In web development, APIs allow clients (like browsers or mobile apps) to send requests and receive data from a server.

## Software requirements

1. [**Visual Studio Code**][vscode] (VScode)
>You will most definitely need some sort of IDE (**code editing platform**). For this guide specifically, [_Visual Studio Code_][vscode] IDE will be used as it is the most common choice.
2. [**Node.js**][node]
>If you already have VScode installed, installing Node.js is a simple task. you can follow [this guide](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
3. Browser
>It is a matter of your choice, whether its [Chrome][chrome], [Firefox][firefox], or [Tor][tor]. You will only need a browser to see how your app looks when launched.

## Express installation
### Once Node.js is installed, follow these steps to install Express:

**1. Initialize a new Node.js project**

Open your terminal and run: 
```sh
npm init -y
```
> This creates a `package.json` file, which manages your project dependencies.

**2. Install Express**
Run the following command to install Express: 

```sh 
npm install express
```
> This will add Express to your project and save it as a dependency.

## Typographical Conventions
To maintain clarity and consistency throughout this guide, we use the following typographical conventions:

1. <ins>**Code Blocks** - Used for commands, code snippets, and examples.</ins>
    
    Ex:
    ```js
    console.log("Hello Express");
    ```

2. <ins>**Inline Code** - Used for small code elements within a sentence.</ins>

    Ex:
    
    _Use the `app.get()` method to define a route._

3. <ins>**Bold Text** - Highlights important terms and concepts.</ins>
    
    Ex:

    **Middleware** functions help process requests before sending a response.

4. <ins>**Italic Text** - Used for emphasis or to introduce new terms.</ins>

    Ex: 

    _Express is a lightweight framework for Node.js_


## Notes and Warning Messages
!!! tip

    Declares a best practice method.
    
    Example: Using req and res instead of request and response
    ``` js
    app.get('/', (req, res) => {
    res.send('hello world')
    })
    ```

!!! danger

    Declares an error/bug or a code vulnerability

    Example: You should not use api/security codes in your code, instead put them in an .env file

    ``` js
    git_api_code = 1234Abc
    ```

!!! success

    Declares a successful completion/ expected result

    Example: If you have done everything right, you should see <123> in your terminal

    ``` js
    console.log('123')
    ```

!!! example

    Declares a non-coding related example

    Example: Describing a folder as a real life folder

    <figure markdown="span">
    ![Image title](https://images.pexels.com/photos/4792284/pexels-photo-4792284.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2){ width="200" }
    <figcaption>Taken from Pexels: [source](https://www.pexels.com/photo/man-opening-blue-briefcase-with-documents-4792284/)
    </figcaption>
    </figure>

!!! note

    Declares a note



<!-- Links *********************************************-->
[express]: https://expressjs.com
[node]: https://nodejs.org/docs/latest/api/documentation.html
[js]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[html]: https://developer.mozilla.org/en-US/docs/Web/HTML
[git]: github.com
[gitGuide]: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
[vscode]: https://code.visualstudio.com
[chrome]: https://www.google.com/intl/en_ca/chrome/dr/download/
[firefox]: https://www.mozilla.org/en-CA/firefox/new/
[tor]: https://www.torproject.org
[api]: https://www.postman.com/api-platform/api-documentation/#:~:text=API%20documentation%20is%20a%20set,of%20common%20requests%20and%20responses.
<!--*****************************************************-->
