# CCI Platform Development Angular 5+ Assignment

## Purpose
At CCI Platform Development  we are passionate about software engineering and cutting edge solutions. We pride ourselves on 
the application of the best solutions for the appropriate problems. We love working with talented and detailed Software 
Developers who also take pride in their work. Our test is very open-ended and non-prescriptive. This is intentional. We 
recognise that different developers have a range of different skills in their toolbox. We'd love to understand what your
talents and skills are and what you believe is important.

## Test Overview

Create an application using Angular which will allow a user to connect to GitHub via an [API](https://docs.github.com/en/rest) client. The application should 
provide the user with the ability to navigate between various features as described below.
 
We will assess your deliverable based on your code neatness, readability, logical flow, visual design and speed. 
All individuals have different strengths so be sure to choose the approach to problem-solving that suits your strengths.

## Use cases:

1. As a User I would like to search GitHub in order to view the available repositories for a given search term

2. As a User I would like to select a particular repository in order to view more details of the selected repository

3. As a user, when viewing a given repository, I should be able to clearly see the URL, description, forks count, stargazers count, open issues count etc

4. As a User I would like to link off to the actual GitHub page where the repository is located in order to view the code in the repository

5. As a User I would like to view a list of all the current issues for a repository in order to view the backlog of issues

6. As a User I would like to filter the list of issues between STATE = ["Open" or "Closed"] in order to look through the filtered list

7. As a User I would like to view a PIE chart that displays the breakdown of issues for the repository (open vs closed) in order to visually see how well built and maintained the repository is



## Additional Points and Notes:

1. Implement the best design possible for the user interface. You are encouraged to make use of interface design solutions 
such as Twitter Bootstrap, Material and any other libraries you may deem necessary to provide your best solution. 
2. Focus on using best practices in writing TypeScript, CSS, and HTML. Write clearly and use proper MVC structure to write 
the application. Show us what your typical standard of work, as well as the kind of standards you want to work to.
3. We have found that the best Software Developers put effort into presentation and ease of use. Provide us not only with a link 
to the repository that houses your solution but include a [README.md](https://en.wikipedia.org/wiki/README) which explains any design choices as well as how to get 
the application up and running on a Windows or Linux machine.



###Distribution:
Once you are done, please upload the application to a repository and give us access so that we can download/view/test it.
Consider how you would setup this repository if a team of developers is going to working on it.

### Delivery
Provide us with a link to an online source code repository after completion.

### Evaluation Criteria:
We should be able to clone the repo / download artifacts and run it without any installation or configuration.

**Relevant Links**

| **Description** | **URL** |
| --- | --- |
| Sample API URL to search by repository name | [https://api.githubwhen given the time to arch/repositories?q=bootstrap](https://api.github.com/search/repositories?q=bootstrap) |
| API URL to display issues of a repository name | [https://api.github.com/search/issues?q=repo:username/reponame](https://api.github.com/search/issues?q=repo:twbs/bootstrap) |
| Example: Display Issues of Bootstrap | [https://api.github.com/repos/twbs/bootstrap/issues?state=all](https://api.github.com/repos/twbs/bootstrap/issues?state=all) |
| API Documentation | [https://developer.github.com/v3/search/#search-issues](https://developer.github.com/v3/search/#search-issues) |
| GItHub Search API Documentation | [https://developer.github.com/v3/search/](https://developer.github.com/v3/search/) |

