---
title: "HSystems setup"
date: 2020-06-08T06:00:23+06:00
hero: /images/posts/writing-posts/analytics.svg
description: Testing my posts
theme: Toha
menu:
  sidebar:
    name: Hyststems
    identifier: Hsystems id
    weight: 500
---



This is a project that relates to a SAGE300 integration between aNewSpring, documentation on this can be found here: [[aNewSpring - Sage]]

# Meeting prep
- Currently in testing stages.
- Assign employees based on role.
	- Can be done via the Admin Portal with some tweaks
- ~~Need to grant access to SAGE servers to HR personal at HSystems~~
- ~~Need to speak with Jono regarding the longevity of test servers for duration of testing by Hsystems.~~ 
- ~~Criteria on Job Title and only certain people.~~ 

Only SAGE Employees
Job title list


# Role based modifications/requirements

## For user -> learner sync.
- Add `Sync.AllowedSyncJobTitle` Table based on `Sync.AllowedSyncCompany` Table.
- Add `Sync.AllowedSyncJobTitle` View based on `Sync.AllowedSyncCompany` View.
- Go one by one through all views where AllowedCompany is inner joined and add inner join for AllowedSyncJobTitle.
	- Can generate entire script for db and lookup from there too. 
## For autosubscription based on role sync.


# Remember! 
- You need to go through Folder publish of dashboard project in Visual Studio to get the files needed to copy onto IIS on the server. 
	![[Pasted image 20240326111000.png|1200]]


H:\Shared drives\IT\IT Admin\Learning Resources\SQL


# NOTES
- OTS codes not being accepting externalDs on aNS. 
- Only list users that are within allowedJobTitle list. 
- Update email templates for ans to better suite C.I 
- Update Zones functionality
	- List of Job Titles instead of Zones
	- Auto Subscribe based on Job Titles
	- 



Portal Logins
admin@newleaftech.co.za
Admin123!


# Notes 2024.05.16

- Look into employee registration and email -> created employee on SAGE but did not get registered on aNS.
- Filter employees by new/active status 
	- Employee Status 
		- Active
		- New
		- Terminated
		- Archived
		- 
- Send Izandi newly filtered employee list - by status and jobtitle 




Filter employee list - by Reinstate new status

### TODO 2024.06.07
 - [ ] Add job title description 
 - [ ] Look at stored procedures for auto subscription 
	 - [ ] Update Code/Views/procedures according to job title instead of by zone 




