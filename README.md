# Hello-world
A hello world application with continuous integration and continuous deployment using GitHub actions as a tool.

# Security vulnerabilities in my approach
Possible security vulnerabilities are:
-Exposure of my heroku token secret which bad actors could use to exploit the pipeline and deployment but I have hidden it using GitHub secrets manager, a secure method utilized by millions of developers.
-Access control to the reepository: Anyone with write access to this public repository can manipulate the pipeline for malicious purposes but write access has been restricted to  the ouner of the respository only (me:-))
-I made use of github actions from the market place which are generally public open source repositories which comes with the general security concerns that comes with open source software as their codebase is open for malicious actors to discover and act on their vulnerabilities but I have made use of GitHub actions that have verified authors by GitHub and/or have a large number of users which usually translate to more support for the codebase to fight against vulnerabilities.
