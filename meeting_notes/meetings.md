# Meeting agendas

A place to put meeting notes.

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
