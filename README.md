# Brickswork (Promo)

### Have you ever taken into account the time during which the system is tested in the project estimate?
Practice shows that for 1 year of development by a small group of developers and with a moderate coverage of the tests of the developed product, the launch of the tests will take about 1 hour. You can object that there are projects where the development is more than 5 years, but the tests take 1 hour. I will tell you that even after 10 years, tests on such a project will take 1 hour. This happens because nobody wants to wait 10 hours for a test cycle, not because there is nothing to cover with tests. A potential regressive danger is hidden in such a project.

_And what if it is possible to create such a framework that will be optimized for testing?_

### How long are you willing to wait for the tests launch?
Functional tests, which are the most common because they cover important nodes well, require the use of a database, and such tests should be run sequentially to avoid competing requests to the database. That is, such testing program code depends on the database.

_But let's imagine that it is possible to emulate the behavior of a database at the level of software code, and then, if you have enough processors on your computer, all the tests can be run in parallel._

### Are you choosing the most popular framework for new projects?
I would say that all the popular frameworks today are oriented towards their popularization by the fact that they can do more than others. This requires constant pursuit of developer qualifications. Yes, it also leads to system flexibility, but is that a plus? And since there is an eternal balance between security and freedom of action, all popular frameworks definitely sacrifice security.

_Maybe it is worth choosing the simplest, but most reliable framework for a new project?_

### Do you start a startup by choosing beginner developers because there are risks?
And another example of optimization of the development process: invite beginner developers to write code and only a few highly qualified ones to correct the direction of work.

_Perhaps it is also worth thinking about a development tool that will be the most secure and reliable. Which could automatically adjust the direction of work through the rules?_

## But what does a simple reliable framework mean?
I propose to describe the following properties:
- _minimum libraries_, which will be considered as easy to use as possible; the functionality of the libraries is reduced to the necessary minimum, which is suitable for any project; the framework depends on the project, not the project on the framework;
- _modular architecture_ of the framework, so that it is convenient to distinguish the area of responsibility of the module and the developers who develop it; full encapsulation of modules so that each module is independent of others and contains functional tests;
- _automatic module validation_ to prevent code duplication; a simple, strictly structured system so that a developer wishing to add new functionality can easily find a place; prevent an alternative implementation without the appropriate permission (rules), but push the developer towards an architecturally appropriate solution;
- _real automatic tests_, that is, these are automatic tests that, thanks to a strict architecture, automatically form test sets for the present modules;
- _minimum dependence on external libraries_; secure integration of third-party code.