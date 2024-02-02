# Meeting agendas

A place to put meeting notes.

- JH = James Hughes
- AL = Anne-Lise Goddings
- DS = Dave Smithson
- SK = Sarah Keating
- KB = Katie Buntic

---

# 02.02.2024

Attendees: JH, AL, DS, SK, KB

# Katie has now joined the project
- Katie will spend some time learning and then move on to the frontend aspects of the app (UI, avatar manipulation, design etc.)

# Similar project at Sussex
- I have asked my colleague to see who the PI is, still waiting for a reply

# Tablets
- JH received the tablet.

# Paying for services
- I have decided to take a simpler approach to deployment,
- So now everything is deployed to AWS including the database and the app hosting,
- This means we don't need to pay for 2 separate services and everything is held in one place,
- This should also make payment easier, I just need the project cost codes,

# Illustrations
- The avatar shadows still need to be investigated,
  - Dave wants to finish off the body types first and then pick up the shadows issue,

# Side on view
- Is it possible to have a side-on version of the illustrations, especially for things like breast development,
- We need to evaluate if we have time and budget for this,
- AL said it would be very beneficial to have this,
- The side-on could just be a contour or outline, might not need to be full-featured (e.g. skin tones etc.),
- Dave will make the illustrations anyway, and then if we have time later in the year we can implement it into the app,
- We can evaluate how we are getting on around March time,

# Meeting schedule
- Dave said he probably will only be able to make every-other weekly meeting,
- Everyone else is with weekly meetings,
- Fine to have smaller meetings in the week if needed too,

# Authentication and authorisation flow
- JH made progress on building the backend to allow researchers to make an account and then create participant accounts,
- Still needs more work but the main concept is working,
- Questions:
  - What data should researchers enter when creating a participant account?
 
# Scripts and content for the app
- AL has been working on the scripts along with her colleague,
- AL will upload the content to a new repo,

# Next steps
- Contine onboarding and training Katie,
- Finish off the backend for opening researcher and participant accounts,
- AL to pick up communications again with the young people,
  - So far we have 2 (both female) who are responding, but we ideally need a male too,
  - SK to ask her contact if he would consider taking part,
- JH to make a new repo for AL to create the content and scripts,
- AL can't make next week,

---

# 19.01.2024

Attendees: JH, AL

JH and AL had a catch up about the current project status and picking up the project again after a brief pause. AL and JH are both happy to keep the project going.

## Onboarding Katie
- AL thinks this is a good idea,
- JH will let Katie know and start the onboarding process so that Katie can start working on some frontend tasks,

## Similar project at Sussex
- JH learned of a very similar project to pubvis currently going on at the University of Sussex
- AL would like to chat to the PI’s about the similar project to see how we might connect,
- JH to get in touch with his contact to start discussions,

## Next steps
- We need to think about form responses and how that might be implemented
    - e.g. have you noticed changes in hair etc.
    - Plan is not to have free text, more likely to be scales and binary etc.
- Need to start thinking about order of events:
    - e.g. start with questions, then show the avatar after,
    - AL to put some docs together,
- Tablets are ready for AL to collect and then send to JH,
- We are still waiting to hear back about an extension
    - Not sure how this might affect our deadlines, preferably we want to stick to our original deadlines,
    - We want to keep on track for the app, but the piloting might be delayed,
- JH to catch up with Dave to see if there is a better date and time that works for him,
    - We could schedule different meetings with Dave to keep progress moving forward,
- AL will get the scripts and order of events sorted and also pick things up again with the young people,

---

# 12.01.2024

Attendees: JH, SK

Apologies: DS, AL

The team couldn't make it again, so we will try to catchup again next week. We could explore the possibility of a pause to the grant until we are all able to continue with the project, JH to ask AL what she thinks about this.

---

# 05.01.2024

Attendees: JH

Apologies: SK, AL, DS

The team couldn't make it today, so we will catchup again next week.

A catchup after Christmas to discuss priorities going forward.

## Documentation
- JH started a doc on the app repo detailing the access control procedures (i.e. how researchers and users will sign up and access the app).

## Next steps
- JH will continue to work on the full implementation for the researcher and user registrations,
  - This means the Illustrations work (from the app side of things) will be on hold for a while,

---

# 08.12.2023

Attendees: SK, JH, DS

Apologies: AL

Shorter meeting as AL wasn't able to make it. So we discussed the latest Illustrations updates and expectations for mid-Jan to have a prototype of the body shapes ready.

## Illustrations
- Illustrations have now been split into male and female,
- Can we remove any old files that are not needed anymore in the Illustrations repo?
  - Answer was yes, let's keep the repo clean.
- The latest version of the .svg doesn't disply quite right in the app. Something with how it was exported?
  - Dave will look into this.
- We need to decide on a file naming strategy,

## AWS solutions architect meeting
- JH had a meeting with an AWS solutions architect. They thought the way the app has been designed so far is very good.
- JH will have a further meeting with an AWS DynamoDB specialist to make sure our implementation is fully optimised.

## App hosting and database costs
- JH doesn't think there are yearly plans for Vercel and AWS,
- Vercel is $20 per month per user, so we can start with just me and see how it goes,
  - Another option would be to have 2 users, one for the main dev (JH) and a backup user if needed,
  - We can deploy the app using AWS amplify if we really need to, it would be a cheaper option but less options and capabilities,
- AWS has a pay-as-you-go pricing model which is why our app costs should be very cheap,
  - If we assume around 100 total users for the pilot then the AWS costs should be very minimal (possibly even close to free),
  - UCL gets a further 12% discount with AWS,
- JH thinks the benefits of using these services does justify the cost. We can always revisit this later if we need to change it,

## Tablets
- Have the tablets been shipped yet? JH will be in Poland from the 9th of Dec until the 30th of Dec,

## Recruitment
- Any latest updates from AL?

## Next steps
- JH will work on the full implementation for the researcher and user registrations,
  - This means the Illustrations work will be on hold for a while,

---

# 07.12.2023

Attendees: AL, SK, JH, Alex Potts

A follow-on from the previous meeting on the 28.11.2023 to discuss data legalities. Overall, Alex is happy with our planned approach to data collection and storage.

## Withdrawal of consent and data deletion
- If a participant withdraws consent, we are not required by law to delete our data in AWS,
  - It's more a question of ethics. We are not legally bound to delete their data, but if a participant requests removal of their data then we may wish to explore this in more detail with the specific user as to whether we can reasonably delete their data or not.
- We need to be clear in our information sheets as to the processes we will adhere to,
 
## Information sheets
- The information sheet and consent process will be handled when the user visits the researcher,
- When the user gets to the app stage, they will then tick a box that says something like: “I have been shown the information and consent forms by the researcher and have agreed to take part...”,
- So the app itself will not be responsible for showing the information and consent forms, it’s assumed they have already been through this with the researcher,

## Terms and conditions of the researcher participation
- Alex said it’s a good idea to inform the researchers about their obligations (e.g. proper handling of the user data),
- Just good in general to make sure the terms and conditions are presented to the researchers,
  - How would this be handled if a new researcher requests an account? Do we send them an information sheet prior to them being 'accepted'?

---

# 07.12.2023

Attendees: JH, Chris Dye (AWS solutions architect)

Meeting with Chris to discuss the technical architecture of the app and get advice.

Overall, Chris was very complimentary about the current architecure and implementation. Everything has been set up nicely and will serve as a solid foundation for the rest of the app.

## Actions
- Chris will set up a meeting with an AWS solutions architect who has specific experience with DynamoDB. So they should be able to give me more specific advice on getting the most out of the service.

---

# 28.11.2023

Attendees: AL, SK, JH, Martin Donnelly, Rob Maughan

A meeting to discuss data governance. Overall, both Martin and Rob were satisfied that our current plan for data storage is satisfactory.

## Martin's thoughts
- It might be a good idea to produce a diagram for transparency of how the data flows from the app to the database. This can be included in the code repo or another documentation location.
- Once data has been anonymised, it is no longer considered personal data.

## Rob's thoughts
- We should include a privacy statement on the login/registration page,
- We need to think about consent and data withdrawal,
  - e.g. do we need a process to handle data removal if a participant withdraws their consent?
- It’s good that we will store the personal data away from the web app data,
- We need to make sure that all of our briefing, information sheets, and consent forms are fully transparent,
- Storing the name and emails of researchers is fine as it’s already probably publicly available,
- We need to make sure the researchers have the ability to reset their password,
  - Rob's preference would be to use Azure SSO to handle authentication, but it's not essential to the project
- Might be good to consider potential alternatives to the Data Safe Haven, but as long as researchers do have a secure enviornment to store data then that's fine.

## Actions
- Martin will introduce us to Alex Potts for a deeper discussion about the legalities of our planned approach.
  - This is mainly as a further precaution and to get the "legal stamp of approval".

---

# 24.11.2023

Attendees: AL, SK, JH

# What devices should the app be used on?
- Tablets, laptops, desktops?
- Making it completely adaptable across all range of devices (e.g. laptops) isn't a priority for the pilot,
- After the pilot, AL wants it to work on a broad range of tablets and computers (e.g. laptops, desktops etc.),
  - But this is for the future of the project,

## App hosting and database costs
- AL would need to use her own credit card for AWS and Vercel as the finance team said they won't cover the costs,
  - AL is still having discussions with the finance team though to see if there is a solution,
  - AL asked if there is an annual cost option (need to investigate), this would be preferable for covering the costs from the grant,
- We need to figure out a long-term solution to this as AL paying for this isn't a good option, 

## Tablets
- JH still needs a tablet to develop and test the app,
- Plan is to order 2 surface pros,
  - We have different screen sizes: 
  - Also various memory sizes,
- We are going to buy 2 tablets that are the same for now (some sort of medium range, medium screen size),
- Hoping to get the tablets before Christmas

## Recruitment
- Ongoing discussions with the youth leader. Questions over whether communications need to funnel through the youth leader or whether direct contact is possible,
- Should be able to navigate this as the participants are all 18+

## App flow
- We decided to go with scenario 1 in the access_control document JH made last week,
- Researchers will make user ID's and passwords for the young people (and store in the DSH),
- Young people will gain access to the app by entering the userID and password,
- AL will write up a detailed document describing the app flow process and upload to github

---

# 21.11.2023

Attendees: AL, DS, JH

A meeting to discuss the technical details of the Illustrations.

## Avatar level of detail
- AL confirmed that we should go with the maximum level of detail (Dave's option 3 illustration),

## Adobe Illustrator workflow
- JH suggested a potential workflow to use in Adobe Illustrator,
- All major elements to be in named layers (e.g. clothes, skin, anaotomy),
- Sub-layers (e.g. paths) to have a reusable `graphic style` so that the layer will be exported with a CSS class name

## BMI
- AL suggested that we ask the user what their approx height and weight is, then present them with 3 potential body sizes/shapes,
- Overall, we would design the following body sizes/shapes (loosely fitting around BMI):
  - Four body sizes: underweight, normal/underweight, normal/overweight, overweight
  - Three body shapes: TBD (potentially something like apple, pear, triangle etc)
  - All of the above combinations duplicated across both male and female avatars
- We avoid extreme body sizes (e.g. very skinny or obese) as these present clinical challenges,
- Dave said he could produce all of the above by early January

## Hair and colour
- We could ask for this information before showing an avatar to avoid biasing choices.
- We could present colour 'swatches' so that users can select the colour that matches them, then confirm it on an actual avatar.

## Zooming
- One idea could be to zoom in on an anatomical feature to allow more precise editing
- JH said that this is a good idea, but we need to manage expectations given the limited budget and timeline,

## Actions
- DS to produce separated SVG's for male and female and upload to GitHub,
- DS to make a start on producing the illustrations for body size/shape,

---

# 17.11.2023

Attendees: AL, JH, SK

## Illustrations
- JH started adding instructions to the Illustrations repo so that our work can be replicated.
- Further work done on developing the best strategy for importing the illustrations into the app and manipulating them via CSS classes,
- Some fiddly work in Adobe Illustrator was required to export custom CSS classes within the SVG,
- Next steps: make a start on refining the SVG's
  - Male and female as separate SVG's but with all the styling attributes kept consistent,
  - Replicate the bottom body layer for both male and female to account for a range of body types/shapes/sizes (how many variations?),
  - Figure out the best layer configuration to give maximum flexibility,

## App hosting and database costs
- App hosting: we still need a credit card to charge the costs against,
- Database: we still need the grant cost codes,
- AL put in a request to the finance manager, not had a response yet,
  - AL could potentially pay for this herself and claim it back later, depends on the finance managers decision,

## Tablets
- JH still needs a tablet to develop and test the app,
- AL ordered them but they got refused, we have now changed provider and reissued the order,
- Currently ordered 2 tablets: one for JH and one for AL,
- Hopefully get a response soon,
- We still need to decide what devices the app should be used on,

## Recruitment
- Got 3 people who want to particiate so far,
- AL sent a brief and initial questionnaire,
- All 3 are female so far but hoping to get more diversity soon,
- All 3 seem very enthusiastic,

## App flow
- We discussed ideas for how the app will function in terms of who can create an account and how young people will gain access to the app,
- We decided that the app will be restricted so that it is not completely open to anyone to make an account (for ethical reasons given the sensitivity of the project),
  - Researchers will request access to the app, and a master admin will grant access or not,
  - Reasearchers with an account should be able to create Users and then share a unique ID with a young person so that they can gain access,
  - Full details to be written up in a separate document,
- We also discussed needing to strike a balance with what is technically possible  given the time and budget constraints. For example, we could build a master admin UI interface to grant user access, but then that is another layer of complexity.

## Information Governance
- JH will set up a meeting between the pubvis team and Martin Donnelly (Head of Data Governance) to discuss data capture and storage in more depth,

---

# 10.11.2023

Meeting cancelled.

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
    - AL said that height and weight proportions are more important than 'age',
    - We should follow up with Dave about how he might depict different age ranges (e.g. a 15 year old),
    - Eventually, the app should be usable by people as young as 9 up to about 15,

# App hosting and database costs
- App hosting: we need a credit card to charge the costs against,
- Database: we need the grant cost codes,
- Now that AL's contract has been sorted we should be able to move ahead with this in the coming weeks,

# Tablets
- JH needs a tablet to develop and test the app,
- Again, now that AL's contract is sorted these should be on order soon,

# Recruitment
- Any updates?

# Other points of discussion
- A no-cost extension should be possible, but we should still aim for the summer 2024 deadline,

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
