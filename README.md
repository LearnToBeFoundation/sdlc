# Software Development Lifecycle at Learn To Be

Despite being a small team, it's still important we develop software the right way. The brief document below describes what we've informally been doing anyways. 

## Steps

1. Product Requirement Document (PRD) - Create a PRD using [this](https://docs.google.com/document/d/1pDMR0-7gIF6o8VZdYONAIRqZWnkJ1ZzRW6ACqcT_7cY/edit#) template

2. Feature approval and ticket creation during sprint planning

3. Feature development and testing

4. Feature QA on staging

5. Feature deploy and monitoring


### Product Requirement Document (PRD)

In lieu of too many meetings, any new product/feature should be have specifications written into the template linked above. All relevant conversation should happen on that document as well. There are a few deliberables from the PRD: 
- is the feature viable
- should we build this feature now and what is the timeline 
- what is the cost of building this feature
- what (roughly) are the tickets that should be created to complete this project

### Feature approval

Product is led by Neeraj so all PRDs should be shared with him for review. If approved, we will slot in tickets to sprint planning, which we host every 2 weeks. 

### Feature development and testing

Tickets are ideally created on separate branches. Branch names should be prefixed by their corresponding Jira ticket number. So, if the ticket you're working on is `LTB-256`, then your branch name should be `LTB-256-<brief-ticket-description>`

All features developed should have unit tests written. And where possible, end-to-end tests should be written as well. 

Open a PR and request a review from at least Neeraj. All code must be approved by at least one other developer. Github actions should also pass before the branch is merged into main. 

### QA testing

Before merging into main, we should have our team QA the feature.

We don't have a formal QA team but you can rely on our program team (Ali, Ashley, Shawn and Michael) to test. Deploy your feature to staging with detailed instructions on how to test the features in question. 

Make sure that the staging database is up to date and all relevant data is seeded so that our program team is able to accurately QA. 

If bugs are found, fix them and ensure test suite is updated appropriately. 

### Feature Deploy

If all looks good and the PR has been approved, merge your branch into main and deploy to Heroku. 