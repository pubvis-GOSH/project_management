# Meeting agendas
A place to put meeting notes ahead of our regular catchups.

---

# 03.11.2023

## App updates
- Now have a skeleton for the app with a working authentication solution,
- Basic writing to a database working based on who is currently authenticated,
- Started work on manipulating the avatar,

## App design input
- I reached out to ISD again to see if help might still be available but have not heard back,
- If we get no response we should probably assume design help isn't available at this time,

## Illustrations
- JH and DS made some technical decisions on the illustrations (e.g. we will use .svg format),
- Go over the design document and make sure that everyone is happy with it,

## User stories feedback
- User story 1:
  - Suggests that the app should have a 'virtual' option so we should consider this,
  - Should we account for different ages of the avatar? e.g. ages 12-13; 13-14; 14-15

# App hosting and database costs
- App hosting: we need a credit card to charge the costs against,
- Database: we need the grant cost codes,

# Tablets
- JH needs a tablet to develop and test the app,

# Recruitment
- Any updates?

# Other points of discussion
- 

---

# 29.09.2023

## Actions from last time
- JH reached out to Samantha regarding design help, but no response yet
- JH decided on a tech stack and possible deployment platforms (NextJs + Vercel or Render.com)
- JH currently working on an auth solution

## Backend running costs
- Discuss backend hosting solutions and running costs,
- Deployment option 1: Vercel, £20 a month but comes with the best options
- Deployment option 2: Render.com, £7 and still good options but maybe not quite as good as Vercel
- Database in AWS: DynamoDb, if the amount of data is relatively small then it will be practically free. 11% discount from UCL

## Custom domain
- Do we want or need one?
- Costs do apply

## Dedicated repo for young participant discussions?
- We could create a separate space for the young participant discussions,
- This might be advantageous to keep it separate from the rest of the work (e.g. code and illustrations)

---

# 15.09.2023
## Image slider prototype
- Go through the prototype app that I made for picking images with a slider,

## User Stories
- I made a document to start off the creation of some user stories. We should go through this together.

## Artist updates
- Scheduled a meeting with Dave for the 20th of September at 12:30pm. Just waiting to hear back.

## GOSH IT updates?
- Are there any updates from the GOSH IT department?
- Difficult to make final technology decisions until we have spoken to them.

## Actions
- James to start thinking about deployment options for frontend, backend, and a database (app user input/results needs to be stored).
  - Also thinking about password protection. We decided the app is fine to be publicly available on the internet as long as it sits behind a password.
- James to get in touch with Samantha Fanning to see if a designer might be able to assist us in mid October.
- Anne-Lise to send James and Sarah a meeting invitation September 25th at 12:30pm

---

# 18.08.2023
## Now using a GitHub organisation
- Go through the features and ideas,
- Talk about the `discussions` feature
    - Not sure if we will use this, but could be a good idea
- Migrated over all issues to the new org

## Initial codebase
- Setup an initial codebase,
- Using React, but that might change if Next.js looks better,
- Using Typescript as this is a more robust and safe way of writing code

## App design
- JH will create a document to outline all the features of the app:
  - e.g. pages, device compatibility etc.
  - Also put some user stories together

## Tablet access
- Are these on order?
- JH to have one for development?

## Github pages
- You can now access the initial webpage,
  - https://pubvis-gosh.github.io/pubvis/
- We can have the staging app here so everyone can access it and play around with it,
- Put it behind a password?
- We could buy a custom domain if needed?

## Artist
- Still need to get in contact with David,

## GOSH IT network
- We need an email address so that I can start talking to them about deploying apps within the network,

## Actions
- JH to make the app design document/user stories,
- JH to decide on final technology to use (React vs. Next),
- Add David to the GitHub org when we start chatting with him,
- AL to provide main contact for GOSH IT department,
