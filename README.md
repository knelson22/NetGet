Netget:
 Data collector that works through browser extension.  for profit.  mysql backend.  will make this closed source project once more developers on board



I did not want to open source this.  I wrote a business plan for this project 2 years ago, then went to grad school.  I’ve been unable to find qualified developers to work with in person, that’s why I’m here.  I originally thought of this through the time I spent working on CRM.  This project is my baby.

Netget’s purpose is to collect any/all useful information from any website.  An example would be a salesman collecting business leads from yellowpages.com.  There are millions of possible uses.  It works by learning the DOM of each site individually.  Netget would ship already knowing the DOM of some key sites.  An important part of It is a point and click engine, that allows the user to teach netget the DOM of any site, without coding knowledge.  The target time for a user completing this on one website is 30 min.  Netget runs as an extension in browsers.  After It learns a site, data collection is automatic.  

The code above is mostly files and business logic for creating an extension in google chrome.  Most of the code is netget’s business logic, a small part is extension overhead.  I found the learning curve for creating a complex extension like this very high.  

There are still a lot of questions to be answered.  For instance, when a user finds the same record on 2 sites what should happen?  That comes down to the question, should there be a table for each different genre like business listings, or for each site.  I decided it would be best for each site to have it’s own table.  The relationship between users and sites would be m-m.  So there’s join table between users and each table to eliminate redundancy.  

Here’s a list of what needs to be done.
•	Extension 
o	Finish parsing extension
o	Develop engine for teaching 
o	Authentication
•	Website
o	Billing system 
o	(Important) develop authentication system 
•	Database
o	Develop structure /complex
o	Conceive relationship for data 

