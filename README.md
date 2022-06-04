
## About

This is a hello world nodejs application that has continuous integration and continuous deployment pipeline setup using GitHub actions. 

### Continous integration

Available test in the respository is a linting test using Eslint and this is the only test ran in the CI stage. I made use of actions/checkout@v3 for this.

### Continous deployment

The codebase is deployed to heroku. Access to the heroku application for deployment was made possible using heroku api keys, heroku account's email address and heroku application's name. I made use of akhileshns/heroku-deploy@v3.12.12 for this.

Live site: https://hello-world-bit.herokuapp.com/

## Security vulnerabilities in my approach
Possible security vulnerabilities are:
- Exposure of my heroku token secret which bad actors could use to exploit the pipeline and deployment but I have hidden it using GitHub secrets manager, a secure method utilized by millions of developers.
- Access control to the repository: Anyone with write access to this public repository can manipulate the pipeline for malicious purposes but write access has been restricted to  the owner of the respository only (me:-))
- I made use of github actions from the market place which are generally public open source repositories. It comes with the general security concerns that comes with open source software as the codebase is open for malicious actors to discover vulnerabilities and act on it but I have made use of GitHub actions that have verified authors by GitHub and/or have a large number of users which usually translate to more support for the codebase to fight against vulnerabilities.

## Possible edge cases

- Heroku token could expire leading to to a failed build.

