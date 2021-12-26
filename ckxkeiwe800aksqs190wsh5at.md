## Static Code Analysis - A Beginner's Guide


Working on a large software project can often be a _challenging_ yet _rewarding_ experience. As a developer, you write code to solve problems. 

However, you’ll have to write secure, bug-free code, and follow best coding practices while complying with standards. And this can be super difficult when you’re working under pressure.
<img src="https://media.giphy.com/media/9DpmqxzBBreVJf3LWH/giphy.gif"> 

This is where **Static Code Analysis** can come in handy.

By the end of this post, you’ll have learned enough to answer the following questions: 

- What is static code analysis? 
- Why should you care about static analysis as a developer?
- What are the advantages and limitations of static code analysis?

## What is static code analysis?
In simple terms, **static analysis**, or **static code analysis** scans your code to identify potential bugs, weaknesses, and anti-patterns—all without actually executing the code.

> So how exactly does static analysis work under the hood?

Well, static analysis often involves _parsing_ of the source code into an _intermediary representation_ on which you can run analysis. This analysis then returns potential security issues, bugs, and performance issues in your code—which you can fix almost immediately.

Now that you know what static analysis is, you’ll learn how it can help you write better code in the next section.

## Why should you care about static analysis as a developer?
As a developer, static analysis helps you in every step of the development process. You can:
- write code, 
- run static analysis, 
- review, and 
- fix reported bugs—without having to wait for code reviews. 

And it’s a lot easier to fix bugs as and when they arise rather than having to regress and do it much later.

Unlike the conventional testing process, where you need a specific module to be all ready to go, static analysis only requires a **chunk of code that can be modeled**. 

The term ‘**modeled**’ here means that the code can be parsed into that intermediary representation on which the analyzer can be run. Please note that your code is never actually run in the process.

This intermediary representation is often the **Abstract Syntax Tree (AST)**. 

If you'd like to know more about ASTs, consider giving this post a read.

%[https://balapriyac.hashnode.dev/abstract-syntax-tree-ast-explained-in-plain-english]


Because of how static analysis can be integrated into development right from the beginning, you can run analysis at every step and make sure your code meets the standards. 

This ensures that your code is almost bug-free when the actual testing process begins.
<img src="https://media.giphy.com/media/L1R1tvI9svkIWwpVYr/giphy.gif"> 


So far, you’ve learned how you can benefit from static analysis as a developer. Let’s put together the advantages in the next section.

## Advantages of Static Analysis
- Static analysis is much faster and a lot more efficient than manual code reviews.
<br>
- The earlier you detect bugs and security issues, the easier it is to fix them. This saves time and substantially _reduces cost_.
<br> 
- Waiting until deployment and then checking for vulnerabilities, regressing, and making fixes is needlessly complex and time-consuming.
<br>
- By shipping software that’s backed by quality code, you build trust, gain and retain customer base. This in turn motivates you to build more helpful products.


![Advantages of static analysis](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6qy6497tarm28t1cql1o.jpg)

Well, are there any caveats yet? Let’s summarize the limitations of static analysis in the next section.

## Limitations of static analysis
- On the flip side, static analysis is prone to **false positives**. The analysis may report too many bugs, some of which may not actually be bugs. 
<br>
- For a large codebase, reviewing each of the reported bugs and vulnerabilities could come across as an overkill. Therefore, running static analysis as you code your way through the project is recommended.
<br>
- Static analysis can **miss** certain **subtle bugs** which require human expertise. But it’s possible to fix them in subsequent steps of code review.
<br>
- And it’s always possible to improve the static analysis tool by embedding this intelligence to identify new bugs—therefore, static analysis is _extensible_ to find new bugs.
<br>

Hope this post helped you get a high-level overview of static analysis, its advantages and limitations. See you all soon in another post!
