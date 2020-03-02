# Auto Integrate Technical Test

Auto Integrate is a web-based ‘real time’ maintenance authorization tool that has been developed specifically for the US and Canadian fleet management service industry.

## Task Rules
The task rules are as follows:

1.	We recommend you don’t spend more than 8 hours on the task.
2.	You are free to use the internet for research, inspiration and help.
3.	Your solution should be your own work
4.	Your solution should be built using a combination of Microsoft C# .NET / C# .NET Core based technologies such as ASP.NET MVC, ASP.NET Web API.
5.	Bonus points if you can demonstrate the use of a front-end framework such as React / Angular / Vue etc.
6.	Your solution should make use of appropriate mocks and stubs for external dependencies.
7.	Your solution should be covered by appropriate tests.

## What Are We Looking For?
This test is designed to help us to understand your experience and technical abilities. We are looking for evidence of the following:

* How you architect your solution
* How you name things
* How you structure your code
* How you isolate and manage potential change

We are really interested in the trade-offs you make, why and we don’t expect the solution to be complete. 

For example, its perfectly acceptable to abstract away data access behind an IRepository interface, but the actual concreate class could make use of an array of static data rather than calling a datastore.

The most important thing is for you to show your level of skill and experience!

## Deliverables
At the end of the task the following **must** be submitted via GitHub (or equivalent):

* A README.md
* A User Interface
* An API

Your solution should demonstrate that you have successfully implemented all the business logic detailed below. It is **very** important that you document your decisions as you will be expected to talk through your approach at interview.

## The Assignment
Your task is to design and build a simple automated job approval system. Your solution should generate a random job sheet and a total price for the work. This job sheet should then be submitted, assessed and a decision returned.

### Business Rules
If any of these rules are broken, then automatically decline the job sheet:

* Tyres must be changed in pairs, and a job sheet can include a maximum of 4.
* Brake pads and discs must be changed at the same time.
* A job sheet can only a include a maximum of 1 exhaust.
* The total hours labour must not exceed the reference number of hours labour.

### Overall Decision
* Approve - If the total price is within 10% of the reference price.
* Refer - If the total price is between 10% and 15% of the reference price.
* Decline - If the total price exceeds 15% of the reference price.

## Reference Data
| Item	      | Unit Time (Mins) | Unit Cost (£)|
| ----------- | ---------------- | ------------ |
| Tyre        |	30	             | 200          |
| Brake Discs |	90	             | 100          |
| Brake Pads	| 60	             | 50           |
| Oil         |	30	             | 20           |
| Exhaust     | 240	             | 175          |

