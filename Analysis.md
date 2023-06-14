# Analysis document
### Stakeholder analysis
[Source](https://fhict.instructure.com/courses/13025/pages/stakeholder-analysis-who-has-a-stake-in-the-project-and-in-the-software?module_item_id=916361)
#### What is a stakeholder?
"A person with an interest or concern in something, especially a business." [Source](https://languages.oup.com/google-dictionary-en/)

#### Who are the stakeholders in your project and what are their goals and constraints?
In my personal project the stakeholders would include: the teachers, future users, me, myself and I.
As I am both the stakeholder and the developer, my goals are developing as many user stories and my constraints would be time and the need to focus on other things besides the user stories.
The teachers' goals are to see me succeed (at least I hope) and to see an end product.
Their constraints would be their role as theacher, because they have to grade my project instead of just being the stakeholder.

##### You have identified and analysed your stakeholders – their goals, constraints, stakes.
In the group project the stakeholders would include: the teachers, future users, future animals, the Finnish development team and our development team.
The teachers' goals are to see an end product. The future users' goals are to be able to use the application. The future animals' goals are to (hopefully) find a forever home. The goals for both development teams would be the same: developing as many user stories and making the application the best ik can be.
The teacher' constraints would include their role as theacher, because they have to grade my project instead of just being the stakeholder. The constraints of both future users and future animals would be whatever they cannot do with the application (as in functionally). The development teams' constraints are time, because time is needed to complete the application.

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Process analysis
[Source](https://fhict.instructure.com/courses/13025/pages/process-analysis-which-processes-are-supported-by-your-software?module_item_id=916362)
#### What is a business process?
"A business process is an activity or set of activities that accomplish a specific organizational goal. 
Business processes should have purposeful goals, be as specific as possible and produce consistent outcomes."
[Source](https://www.techtarget.com/searchcio/definition/business-process)

#### How does a business process relate to software applications?
Software development is a rapidly changing field and with those changes comes changes in the BPM (Business Process Manegement).
These changes in BPM are than adapted by other fields and slowly change into the standard. 
So the development of software applications help improve BPM, thus you could say that a business process relates to software applications by means of improving with new developments being made in the field of software. 

[Source](https://itchronicles.com/business-process-management/business-process-management-in-software-companies/)

#### Context
(Wat houdt het zichtbare proces in? Waarom moest het aangepast worden? Wat is het verschil tussen het oude en nieuwe proces?)

I write this business process analysis about a user story that isn't implemented in my application. This means that the situation setup will be fictional and does not relate to my current application.  

"As a admin I want to be able to see which users added which information, because than the admin can flag users spreading misinformation." 
This is the user story for which I will visualise the business process. 
The Admin needs to be able to look at the information that is stored in the database. That information is currently only available by opening the database, opening the data table and scrolling down the list of changes made. This process is time consuming and it would be much better to have an dedicated page for this (only accessible for the Admin(s)). 
The new process will enable Admins to find problematic comments easier, which means that banning users who repeatedly post misinformation will be easier also. 

#### Process then
(Hoe zag het proces er in het verleden uit?)
![BP_DiveSpot drawio](https://github.com/S3-Portfolio/General/assets/93527848/e460e2e3-6515-47e1-bed3-69f088452dd8)

You can see the old process above. When an Admin wants to know which user posted/edited which information, they have to open the database. They then have to open the table where all changes to the website are stored. Then they have to scroll through all rows, searching for the particular change that they are concerned about. Then they have to change the boolean "Flagged" to true manually. This is very inefficient and time consuming. 

#### Analysis
(Wat kan er in het oude proces verbeterd worden?)

This process is (like previously stated) inefficient and time consuming. The Admin also needs to rewrite queries if they want to flag multiple users (if they wrote a query to search the data faster). This means that this process can be approved immensly to make this task easier.

#### Process now
(Hoe ziet het proces er nu uit?)
![BP_DiveSpot_new drawio](https://github.com/S3-Portfolio/General/assets/93527848/efe10c72-2f45-4e05-aa25-1d6ccb7025ae)

You can see the new process above. When an Admin wants to know which user posted/edited which information, they open the "Changes" page (if they are already logged in as Admin). On the page they will see a table with all changes made to the website and which user posted/edited what. Here they can filter by user (if they want to check if this user should be banned) or by term (if they want to check that there is no problematic language used). Then they check the checkbox next to the user to flag them. This also means that the Admin can flag multiple users at a time.

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Requirements analysis
[Source](https://fhict.instructure.com/courses/13025/pages/requirements-analysis-what-do-you-have-to-make?module_item_id=916363)
#### What are non-functional requirements?

"A non-functional requirement (NFR) is a requirement that specifies criteria that can be used to judge the operation of a system, rather than specific behaviours."
[Source](https://en.wikipedia.org/wiki/Non-functional_requirement)

#### How do you specify functional and non-functional requirements in your agile method and how do you validate them?
Specifying functional and non-functional requirements in agile requires creating SMART user stories, defining acceptance criteria and prioritizing requirements. Validating functional and non-functional requirements in agile requires conducting regular reviews and walkthroughs, testing the user stories, and establishing a continuous feedback loop between the development team and the stakeholders. 
Non-functional requirements should be treated as user stories and written with the same level of detail as functional requirements.

[link.springer.com](https://link.springer.com/chapter/10.1007/978-3-030-67084-9_6) ,
[researchgate.net](https://www.researchgate.net/publication/353752219_Managing_non-functional_requirements_in_agile_software_development)

#### When do you elicit and specify the requirements in your agile method? Are you allowed to change or update them?
Requirement elicitation and specification are continuous processes in agile software development that are done collaboratively with the stakeholders in an iterative and incremental manner. Requirements can be changed or updated throughout the development lifecycle in response to feedback from the stakeholders, changes in the business environment, or new insights gained during the development process. Changes to requirements are documented in the requirements specification and communicated to the stakeholders to ensure that everyone is on the same page.

[techtarget.com](https://www.techtarget.com/searchsoftwarequality/tip/7-techniques-for-better-Agile-requirements-gathering) ,
[t2informatik.de](https://t2informatik.de/en/blog/requirements-specifications-in-an-agile-environment/)

##### You have contributed to the requirements collection and elicitation.

##### You have contributed to the translation of the requirements to User stories.

##### You have contributed to the translation of the requirements to the project architecture and designs.
------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### Project:
* What are the non-functional and functional requirements in your project?

* How did you come up with them?

I had already thought of my idea (what kind of website I wanted to create). So then it became a question of how. An important part of the how question is: What do I need? So thats exactly where I started.

* How and where did you specify and validate them?

I specified my requirements by ...

I validated my requirements by asking feedback from my teachers. This feedback can be read back on FeedPulse canvas. 

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Ethics analysis
[Ethics document](https://github.com/S3-Portfolio/General/blob/ff59881171e8ffb3f35be817bea1122dc8eff051/CulturalDifferencesEthics.md)
