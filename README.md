# Postman API Automation Integration With Github Actions #

This repository is a demonstration for POC for integrating postman tests with github actions.The Tests are written in postman and they are excuted on the VM with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project excution on every push to the main branch.you can also excute the project manually using workflow_dispatch.th projects run on a scheduled time with the help of the cron job.

The HTML report is archieved and kept in the artifact section for the team to download it.Along with that they can view the report directly from the github page:https://poojadeevi19.github.io/Phoenix-Inwarranty-Flow/.
The latest report is mailed to the team members using GMAIL SMTP.

# About Me #
 Hi , My name is pooja .I have 3 years of experience in manual testing & Automation testing. My skillset includes UI, Automation with selenium Webdriver and for api testing i used postman  
 You can connect me over: 1

# Testing Coverage #
1.Happy Flow Testing
2.Negative Testing and Edge case testing
3.Token Testing
4.Data Driven Testing
5.Schema Validation
6.Secrets Management with github Secrets

# Team Stack #
1.Postman
2.Nodejs 22v
3.Newman
4.Newman-Repoter_Htmlextra
5.Github Actions
6.Gmail SMTP
7.Github Pages
8.CSV for Data Driven Testing
AWS-EC2 instance for Self hosted github runner.

# Github Pages #
You can directly view the latest test report of the Postman Test at the Github page: https://github.com/poojadeevi19/Phoenix-Inwarranty-Flow

# HTML Report #   
The Report Will be created in the newman folder
![Postman Report](https://github.com/poojadeevi19/Phoenix-Inwarranty-Flow/blob/static-content/Newman%20report.png)

# Project Structure #
```
Phoenix Inwarranty Flow
├─ Inwarranty-flow collection.postman_collection.json #  Collection File
├─ QA.postman_environment.json # Environment File
└─ testdata.csv # TestData File

```

# How to run the project #
You can run the project on your local system for that 
1. Clone the project on local system https://github.com/poojadeevi19/Phoenix-Inwarranty-Flow.git
2. Install Ndejs and NPM from https://nodejs.org/en
3. Install newman using npm install -g newman
4. Install Newman-repoter_Htmlextra npm install -g newman-reporter-htmlextra
5. Run the newman command:
   
        ```     newman run "Inwarranty-flow collection.postman_collection.json" \
            -e QA.postman_environment.json \
            -d testdata.csv \
            -r cli,htmlextra \
            --reporter-htmlextra-export newman/index.html ```
       
 




