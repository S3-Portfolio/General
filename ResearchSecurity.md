# Research
------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Introduction
(Give a short rundown of why I ask the question)

I am writing this research paper because I want to know which security concerns my application has.
My application is a website for divers to get an overview of diving locations and fish. Have an interactive world map that shows diving locations that are clickable. When clicked show information about dive and fish at that location. Have a search function for both dives and fish. Dive listing shows information about that dive and which fish a diver would be able to see when taking that dive. Fish listing shows information about that fish and which diving locations a diver would be able to see that fish at.

#### Methods
(What methods do I use to research this topic?)

There are a lot of different methods for researching. 
The main ones are: 
* Observation / Participant Observation
* Surveys
* Interviews
* Focus Groups
* Experiments
* Secondary Data Analysis / Archival Study
* Mixed Methods (combination of some of the above)

Of these methods I will mainly use Secondary Data Analysis / Archival Study, but I would also like to gather information through other people.

#### Execution
(How did I execute this method and research?)

I searched on internet and our school courses for information. 
I also discussed this topic with a teacher and fellow students to gathered information through that. 

#### Premise
(Give a short rundown of what my application entails)

I looked at the Canvas course [^1] that gave information about security and which types of security concerns there are. I looked over the list and tried to guess which of these security concerns my application would have. The most likely security concern (in my opinion) that my application would have is "Identification and Authentication Failures". [^2] Because my application enables users to add information to my website for other users to see.
So that is the reason for this research paper.

My objective will be to gather information about security and have a basic understanding about different security issues. I also want to know which security concerns would come up from my application. 

So my main question would be: How can I prevent identification and authentication failures in my application?

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Why would my application have identification and authentication failures?
There are a few scenerio's where identification and authentication failures could come up. 
For my application these would be;
* Permits default, weak, or well-known passwords, such as "Password1" or "admin/admin".[^2]
* Uses weak or ineffective credential recovery and forgot-password processes, such as "knowledge-based answers," which cannot be made safe.[^2]
* Uses plain text, encrypted, or weakly hashed passwords data stores (see A02:2021-Cryptographic Failures).[^2]
* Has missing or ineffective multi-factor authentication.[^2]
* Reuse session identifier after successful login.[^2]
* Does not correctly invalidate Session IDs. User sessions or authentication tokens (mainly single sign-on (SSO) tokens) aren't properly invalidated during logout or a period of inactivity.[^2]

My application would implement security by way of hashing passwords when stored in the database and working with sessions.
This isn't enough to make my application secure, but the most important thing to ask is; How secure should my application be?

Because my application only uses a login system for keeping track of which user makes which changes, there really isn't that much critical user information I need to make secure. For the user experience it would obviously feel better if I (in this case the user) knows that not just anyone can see what I did or didn't type. 
But because admins get to see all (relevant) user information, there needs to be some security. This security will be devided between two subcategories: login and traceable user security.

#### Login security
The most important aspect of login security for my application would be: protecting the login information of users, but most importantly admins. The user login has to be secure, because otherwise an user could change something on the website with the account of another user. This could result in the victim user getting flagged or in the worst case banned. I would obviously want to prevent this to better the user experience.
The login security for the admins need to be more secure, because admins can see some user information and have the authority to flag and ban users. This shouldn't be abused or be accesible to just anyone. For the users hashing passwords would be a good first step, but the admin login information should be secured through more steps. 

#### Traceable user security
(Explain traceable user security issue)


### Prevention of identification and authentication failures
(How will I implement the solutions?)

(deelvragen niet kopjes maken / wat is er nodig om hoofdvraag te beantwoorden? Ook per deelvraag methode noemen en resultaten valideren)

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Results
(What are the results of this research?)

### Conclusion
(What is the conclusion of this research?)

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### References
(Link all used references here. Use footnotes to reference sources)

[^1]: [Canvas](https://fhict.instructure.com/courses/12992/pages/secure-web-development?module_item_id=911584)
[^2]: [OWASP](https://owasp.org/Top10/A07_2021-Identification_and_Authentication_Failures/)
