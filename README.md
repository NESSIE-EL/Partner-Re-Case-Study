Goal of the Case Study 
The purpose of this case study is to give a sense of the types of situations we expect the intern to manage, and the way we collaboratively find solutions through discussion.   
Procedure 
You should receive this case study 2 days before your interview. Please get familiar with the tasks and prepare in advance of the interview, a demonstration following these guidelines: 
•	Use a recent version of R and packages to reproduce results. 
•	Focus on using tidyverse packages (e.g. dplyr and tidyr for data manipulation and ggplot2 for visualization).  
•	Please approach the data set in a critical manner. Apply and document your assumptions where/if necessary. Please be prepared to describe and justify the steps you’ve taken. 
For the situation  
•	Expect us to walk through your code together and ask questions on it. 
•	Be prepared to analyze the data and modify some of your code interactively.  
•	Ensure that you can share your screen (via MS Teams) so we can follow live during the interview. 
Please submit any clarifying questions you may have on the case study by email within 24 hours from receipt and we will respond within 24 hours. 
Situation  
Welcome to the Centralized Pricing Team (CPT)! The team is at the forefront of ensuring fair and competitive pricing for our products and services. Our day-to-day work includes setting benchmarks, reviewing most significant deals, building, and maintaining actuarial pricing tools.  
At the heart of our operations, we collaborate closely with actuaries across all our markets, providing essential support to streamline their tasks and enhance decision-making processes globally.  
In PartnerRe, data analysis and modelling are crucial to understanding our business and adding value to our clients. This is a fast-paced environment, where changes need to be deployed relatively quickly while keeping high standards of delivery. Additionally, we continuously invest in and expand our R-centric Pricing and Analytics Platforms to provide state-of-the-art solutions and capabilities.  
This environment also supports a continuously growing palette of in-house models and tools which have been developed by our actuaries and data scientists. These applications are often specific to a project, or a task and the workflow is generally based on the input-process-output pattern. 
 	1/2
 
Technology stack 
Our well-established technology stack is centered around the following Linux environment:  
•	Git repository with issue tracking & CI/CD pipeline support (GitLab) 
•	RStudio servers 
•	Shinyproxy server hosting dockerised Shiny applications  
•	Docker image repository 
Problem  
In this case study, you are given an in force portfolio of life insurance policies written by a certain insurance company. Unfortunately, it is a new cedant that is not able to provide historical claims data. All you have available is a snapshot of the current portfolio. PartnerRe is quoting to write a new portfolio of another 10’000 policies. Your task is to perform explanatory analysis of the data and simulate the new portfolio 1 year into the future to estimate possible claim scenarios and financial outcomes.  
The sample data file is attached in the case study. Data consist of 3 columns: Gender of insured person, Sum At Risk (SaR) amount (the benefit amount paid in the case of death) and FinalRate (the probability of a person dying within the next year). 



Task 1 – understand the data
The data may need cleansing and/or wrangling before it becomes usable for further analysis.
Please use R to get insights into the portfolio files and modify them so that they will be ready
to use.
Please walk us though your code and the changes you’ve made to the data and explain the
potential impact of your assumptions. Think about the most efficient way to address these
kinds of data issues in the future.

Task 2 – project the portfolio
Use stochastic methods to project the deaths arising from the new 10’000 policies portfolio
within next year. Please explain your approach and analyze your results. How would you
describe and quantify the risks associated with the portfolio? How would you think about
setting a premium rate which PartnerRe can charge to cover this portfolio over the next year?

Task 3 – build Shiny application (prototype) & present your results in visually
“attractive” form that can be presented to a non-technical audience.
Please create a Shiny application that allows for:
1) Ingestion of the cleansed files
2) Preview of the high-level summary of the data (e.g. means, medians, distinct values)
3) Preview of dashboards illustrating sum insured distribution
Please try to touch on each of the points above. Please be prepared to discuss pros and cons
of your solutions and different approaches and discuss how would you like to improve the
code further. Finally, which design choices would you make to minimize time to production
and ensure re-usability of your code, for example in other Shiny apps?
