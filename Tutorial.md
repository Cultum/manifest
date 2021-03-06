## Table of Contents
-  __GIT__
    - [GIT Flow](/sections/git/gitflow.md)
    - [GIT naming](/sections/git/gitnaming.md)

-  __GraphQL__
    -  [GraphQL design](/sections/graphql/graphql.md)
-  __Project structure Practices__
    - [Structure your solution by components](/sections/projectstructre/breakintcomponents.md)
    - [Layer your components, keep Express within its boundaries](/sections/projectstructre/createlayers.md)
    - [Wrap common utilities as npm packages](/sections/projectstructre/wraputilities.md)
    - [Separate Express 'app' and 'server'](/sections/projectstructre/separateexpress.md)
    - [Use environment aware, secure and hierarchical config](/sections/projectstructre/configguide.md)

-  __Error Handling Practices__
    - [Use Async-Await or promises for async error handling](/sections/errorhandling/asyncerrorhandling.md)
    - [Use only the built-in Error object](/sections/errorhandling/useonlythebuiltinerror.md)
    - [Distinguish operational vs programmer errors](/sections/errorhandling/operationalvsprogrammererror.md)
    - [Handle errors centrally, not within an Express middleware](/sections/errorhandling/centralizedhandling.md)
    - [Document API errors using Swagger](/sections/errorhandling/documentingusingswagger.md)
    - [Shut the process gracefully when a stranger comes to town](/sections/errorhandling/shuttingtheprocess.md)
    - [Use a mature logger to increase error visibility](/sections/errorhandling/usematurelogger.md)
    - [Test error flows using your favorite test framework](/sections/errorhandling/testingerrorflows.md)
    - [Discover errors and downtime using APM products](/sections/errorhandling/apmproducts.md)
    - [Catch unhandled promise rejections](/sections/errorhandling/catchunhandledpromiserejection.md)
    - [Fail fast, validate arguments using a dedicated library](/sections/errorhandling/failfast.md)

-  __Code Style Practices__
    - [Use ESLint](/sections/codestylepractices/eslint.md)
    - [Node.js Specific Plugins](/sections/codestylepractices/nodeplugins.md)
    - [Start a Codeblock's Curly Braces on the Same Line](/sections/codestylepractices/curlybraces.md)
    - [Don't Forget the Semicolon](/sections/codestylepractices/semicolons.md)
    - [Name Your Functions](/sections/codestylepractices/namefunctions.md)
    - [Naming conventions for variables, constants, functions and classes](/sections/codestylepractices/namingconvention.md)
    - [Prefer const over let. Ditch the var](/sections/codestylepractices/letconst.md)
    - [Requires come first, and not inside functions](/sections/codestylepractices/firstrequires.md)
    - [Do Require on the folders, not directly on the files](/sections/codestylepractices/notdirectlyrequirefiles.md)
    - [Use the `===` operator](/sections/codestylepractices/strictequality.md)
    - [Use Async Await, avoid callbacks](/sections/codestylepractices/asyncawait.md)
    - [Use Fat (=>) Arrow Functions](/sections/codestylepractices/fatarrow.md)

-  __Testing And Overall Quality Practices__
    - [At the very least, write API (component) testing](/sections/testingandquality/.md)
    - [Detect code issues with a linter](/sections/testingandquality/.md)
    - [Carefully choose your CI platform (Jenkins vs CircleCI vs Travis vs Rest of the world)](/sections/testingandquality/citools.md)
    - [Constantly inspect for vulnerable dependencies](/sections/testingandquality/.md)
    - [Tag your tests](/sections/testingandquality/.md)
    - [Check your test coverage, it helps to identify wrong test patterns](/sections/testingandquality/.md)
    - [Inspect for outdated packages](/sections/testingandquality/.md)
    - [Use docker-compose for e2e testing](/sections/testingandquality/.md)
    - [Refactor regularly using static analysis tools](/sections/testingandquality/refactoring.md)

-  __Going To Production Practices__
    - [Monitoring!](/sections/production/monitoring.md)
    - [Increase transparency using smart logging](/sections/production/smartlogging.md)
    - [Delegate anything possible (e.g. gzip, SSL) to a reverse proxy](/sections/production/delegatetoproxy.md)
    - [Lock dependencies](/sections/production/lockdependencies.md)
    - [Guard process uptime using the right tool](/sections/production/guardprocess.md)
    - [Utilize all CPU cores](/sections/production/utilizecpu.md)
    - [Create a ‘maintenance endpoint’](/sections/production/createmaintenanceendpoint.md)
    - [Discover errors and downtime using APM products](/sections/production/apmproducts.md)
    - [Make your code production-ready](/sections/production/productoncode.md)
    - [Measure and guard the memory usage](/sections/production/measurememory.md)
    - [Get your frontend assets out of Node](/sections/production/frontendout.md)
    - [Be stateless, kill your Servers almost every day](/sections/production/bestateless.md)
    - [Use tools that automatically detect vulnerabilities](/sections/production/detectvulnerabilities.md)
    - [Assign ‘TransactionId’ to each log statement](/sections/production/assigntransactionid.md)
    - [Set NODE_ENV=production](/sections/production/setnodeenv.md)
    - [Design automated, atomic and zero-downtime deployments]()
    - [Use an LTS release of Node.js](/sections/production/LTSrelease.md)

-  __Security Practices__
    - [Embrace linter security rules](sections/security/lintrules.md)
    - [Limit concurrent requests using a middleware](sections/security/limitrequests.md)
    - [Extract secrets from config files or use packages to encrypt them](sections/security/secretmanagement.md)
    - [Prevent query injection vulnerabilities with ORM/ODM libraries](/sections/security/ormodmusage.md)
    - [Collection of generic security best practices](/sections/security/commonsecuritybestpractices.md)
    - [Adjust the HTTP response headers for enhanced security](/sections/security/secureheaders.md)
    - [Constantly and automatically inspect for vulnerable dependencies](/sections/security/dependencysecurity.md)
    - [Avoid using the Node.js crypto library for handling passwords, use Bcrypt](/sections/security/bcryptpasswords.md)
    - [Escape HTML, JS and CSS output](/sections/security/escape-output.md)
    - [Validate incoming JSON schemas](/sections/security/validation.md)
    - [Support blacklisting JWTs](/sections/security/expirejwt.md)
    - [Limit the allowed login requests of each user](/sections/security/login-rate-limit.md)
    - [Run Node.js as non-root user](/sections/security/non-root-user.md)
    - [Limit payload size using a reverse-proxy or a middleware](/sections/security/requestpayloadsizelimit.md)
    - [Avoid JavaScript eval statements](/sections/security/avoideval.md)
    - [Prevent evil RegEx from overloading your single thread execution](/sections/security/regex.md)
    - [Avoid module loading using a variable](/sections/security/safemoduleloading.md)
    - [Run unsafe code in a sandbox](/sections/security/sandbox.md)
    - [Take extra care when working with child processes](/sections/security/childprocesses.md)
    - [Hide error details from clients](/sections/security/hideerrors.md)
    - [Configure 2FA for npm or Yarn](https://medium.com/@oprearocks/eslint-backdoor-what-it-is-and-how-to-fix-the-issue-221f58f1a8c8)
    - [Modify session middleware settings](/sections/security/sessions.md)
    - [Avoid DOS attacks by explicitly setting when a process should crash]()
    - [Prevent unsafe redirects](/sections/security/saferedirects.md)
