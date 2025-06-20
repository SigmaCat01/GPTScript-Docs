Welcome to GPTScript
=============================================

GPTScript is a minimal scripting language that looks like polite chatbot dialogue. It supports basic features like variables, printing, functions, and HTTP requests.

.. contents:: Table of Contents
   :depth: 2
   :local:

Syntax
------

**Variable Storage**

For numbers,

    Let me store the number 42 as answer.

Or for strings,

    Let me store the text "Hello" as greeting.

**Printing**

    Now, let's kindly display: answer

**HTTP Requests**

For GET,

    I would like to fetch from "https://api.example.com" and store it as data.

Or for POST,

    Kindly post to "https://api.example.com/data" with the content:

    {
        "name": "GPTScript"
    }

    .. note::

       The POST request body must be valid JSON. The compiler doesn't care about the way you write it.

**Function Definitions**

    With all due respect, define greet:

    Now, let's kindly display: greeting

    End definition.

    Please invoke greet.

**Program End**

    Thank you for your patience.

Errors
------

* ``WrongUsage`` — Raised when the script isn't passed exactly one ``.gpt`` file as an argument.
* ``ScriptNotFound`` — Raised when the specified script file doesn't exist.
