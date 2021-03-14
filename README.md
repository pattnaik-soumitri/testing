## L2 or Above

1. Tell us about your project and your roles and responsibility in that project.

    <ins>**About Project**</ins>

    Currently I am working on a healthcare application named *Caren*. 
    In th United States, there are more than 49% of families where both married-couples are working. In such families it becomes difficult for the couples to take care of their elders (parents, grand parent, in laws etc.). 
    To solve this problem US has many home healthcare providers called **hospices**, for the elders to live.
    Hospices have trained professionals called care givers who usually take care of the elderly person(s).
    In the Unites States more than 70% of the people older than 60 years are having at least two health conditions, so it becomes extremely important for the hospices to provide means to start or continue diagnosis, monitor the vitals (etc) for the elders.
    
    That's where Caren comes into the picture. In Caren the caregivers or the elders themselves (elders are called **Patient** in Caren) use our apps (mobile and web) to :
    - Track patient's vitals such as BP, Glucose level, SpO2 level, Body temperature, Pain level etc.
    - Manage meals and medication timings.
    - Track health conditions, observations, side effects, Emergency Room Visits, Vaccinations etc.

    Caregivers or the patients themselves can enter their readings and observations and doctors and other family members of their family can monitor their loved ones in Caren.
    
    <ins>**Mention the followings if asked for more details**</ins>

    - Caren also has **Interoperability** where it can automatically sync readings for patients who are using *iHealth* or *Omoron* health care devices (iHealth and Omoron are health care device manufacturer).
    - We are currently working EHR (Electronic Health Record) interoperability. We are currently working with **Cerner EHR** where doctors / hospitals using Cerner EHR can have their patient's vitals and observations being taken and synced to the EHR seamlessly from home using Caren app.
    - We have functionality in the app to manage legal documents such as insurances, wills etc.
    
    <ins>**Roles & Responsibilities**</ins>

    Goes here

1. So you developed the framework or you just work on existing framework?

1. Which methodology you use in your framework? Why?

1. Explain BDD, TDD.

1. Explain your framework structure/modules.

1. Explain your framework execution flow.

1. What is page object model?

1. How you use those objects in your test scripts?

1. How you generate reports?

1. How you generate logs?

1. You just told that you use java in your project, for what propose you use java?

1. You just told that you use selenium in your project, for what propose you use selenium?

1. You just told that you use testNG in your project, for what propose you use testNG?

1. You just told that you use cucumber in your project, for what propose you use cucumber?

1. You just told that you use maven in your project, for what propose you use maven?

1. How you inject dependencies in your framework? You add .jar files or you inject in to your POM.xml file?

1. What plugin or dependencies you use in your frame work?

1. How you test or build or run your automation framework?

1. What tools you use for CI-CD?

    **Jenkins**
1. Can you just explain your ci-cd flow?

    We use Jenkins for automatic and manual build and deployments.
    We have mainly three important branches for our source repositories i.e. `master`, `staging` and `test`.
    When a developers gets assigned to a JIRA ticket (lets say `IA-100`), they create feature (`feature/IA-100`) branches from the `test` branch.
    Then the developer makes code changes for the ticket, does testing on the local then pushes the code to the feature branch.
    As soon as code is pushed to a feature branch, Jenkins automatically create a build from that feature branch (`feature/IA-100`) and deploys that to the `DEV` server.
    Then the developer performs functional testing on the DEV environment. If all look good, then he creates a PR from the feature branch to the `test` branch (`feature/IA-100` --> `test`).
    Then the PR gets peer reviewed by the other developers and finally the developer merges it to the `test` branch.
    As soon as there is any new code change to the `test` branch, Jenkins automatically creates a build from the `test` branch and deploys that to the `TEST` environment.
    At that point the ticket is *Ready For QA*. We perform QA testing on the `TEST` environment and if found a bug it is raised and the same process is continued.
    Once the feature is completely tested, the QA person creates a PR from `TEST` branch to `staging` branch (`TEST` --> `staging`).
    Just like before, as soon as the code is merged to `staging` branch, the build is created and deployed to `STAGING` environment.
    Regression and UAT is performed on the `STAGING` branch and finally a PR from `staging` branch to `master` is created, merging which automatically builds and deploys to `PRODUCTION` environment.

1. You use Jenkins? Can you configure with your framework? 

    Yes, I use Jenkins.
    We have Jenkins auto triggers to automatically build and deploy to different environments when code is pushed / merged to different branches (explained in the above question).
    I use Jenkins to manually build and deploy.
    It is a two step process.
    1. Build
    2. Deploy

    To build I go to the build job, put the branch name which I want to build as parameter and click on build.
    This will create a build out of the source code.
    To deploy, I just go to the deploy job, select the environment from the parameter drop down, put down the build number to the parameter and click on 'Build'.

    I don't know how to configure Jenkins, that is something our DevOps team does.

1. What is difference between `src/main/java` and `src/test/java`?

1. Where from you getting the test data, you use excel, csv or database? How?

1. Do you follow agile? How?

1. Who you report your issues?

1. How and where you report a bug or error?

1. So you mentioned in your resume you are involved in Test Planning , Story analysis  can you explain what is your contribution to  Test Planning , Story analysis .

1. So you have written scenarios, test case and steps, can you explain with an example you have written for your project?

1. So you have written scenarios, test case and steps, I am giving you a webpage for a login function, please tell me what you will write.

1. What are the challenges faced in your project?

1. The challenges you just told us can you explain how you handled or tackled, with an example.

1. What is your team size? What is your roles and responsibility?

1. Who are the team members?

1. What you do if a merge conflict raises?

1. On the day one of joining a company what will your approach as an automation tester? You directly write automation script, you write test cases?

