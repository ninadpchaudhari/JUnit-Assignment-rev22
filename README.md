# Junit Assignment
## Project Description

The Repository contains a maven project with queue extended from [Princeton's Intro to programming](https://introcs.cs.princeton.edu/java/43stack/) sample.

**The problem:** The "enqueue" method has a bug : The developer has forgot to throw an exception when the queue is full.

**The Task**: As a Software Tester, Write junit test cases for this project to reveal
this fault and also to test all functions of the Queue Class which should result
in 100% code coverage for this class.
#### Current code coverage: 
![Instructions Coverage](.github/badges/jacoco.svg "Instructions Coverage Jacoco")
![Branch Coverage](.github/badges/branches.svg "Branch Coverage Jacoco")

## Requirements for assignment

* Have 100% instruction & branch coverage for both constructors, enqueue, dequeue, peek, length, isEmpty, removeAll for Queue Class.

* Order of test execution cannot be manually set. Tests can be run indepedenly of each other.
* Annotations of JUnit are to be used.
* You should have atleast 1 failing test which reveals the bug in the enqueue method disclosed earlier.
## Instructions for submission

* This repo should already exist as a base code in your particular Github Classroom repositories, push your changes to your respective repositories.
* Submit a compressed file of the entire project which contain the reports already generated.
## Instructions to run
You can check the current code coverage using the following ways:
### Checking code coverage on local machine.
To Run tests and generate coverage reports :

> mvn jacoco:prepare-agent test jacoco:report
or just 
> mvn test
* Location of reports : *target/site/jacoco/index.html*
* [Screenshot of a sample report](https://github.com/ninadpchaudhari/JUnit-Assignment/blob/master/jacoco-report-sample.png?raw=true) 

### Automatic Coverage test: 
This repo is configured to automatically generate a new commit after you push code online!
This commit will generate badges reflecting the current test coverage of code.
You can just push code to github then wait for the github action to finish
which should update the badges automatically! 

*Please do `git pull` after the bot has updated your repo with badges*
This helps everyone stay on the same page.


#### References
* [JUnit 5 User Guide](https://junit.org/junit5/docs/current/user-guide)
* [JUnit 5 Samples](https://github.com/junit-team/junit5-samples)
* [JUnit 5 tests for *Stack*](https://github.com/junit-team/junit5/blob/master/documentation/src/test/java/example/TestingAStackDemo.java)
