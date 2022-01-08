## Goal:

This task is the data collection process of my research project, which studies the geographical wage gap of the remote workers on Upwork. For this task, I need someone to:

1. Write two scripts.
	- One script that scrapes the profile page link (like [this](https://www.upwork.com/freelancers/~01ca3ec01c6f84d3df)) from the first 100 profiles (10 pages) of [Freelancer Search Results - Upwork](https://www.upwork.com/ab/profiles/search/?category_uid=531770282584862721&occupation_uid=1017484851352698921&user_pref=1). Please see the profile link section for a detailed description of profile data. Output the result to Json. 
	- One script that scrapes the profile data in these [profile pages](https://www.upwork.com/freelancers/~01ca3ec01c6f84d3df). Please see the profile data section for a detailed description of profile data. Output the profile data of each worker to Json. 
2. Complete the work above within 7 business days. 

### Essential Requirement:

You need to be familiar with some anti-scraping techniques because Upwork encodes worker profile data, as shown in the source code of [this page](https://www.upwork.com/freelancers/~01ca3ec01c6f84d3df). 

### Potential Resource: 

[Upwork Scraper · Apify](https://apify.com/trudax/upwork-scraper) allows users to scrape a limited amount of variables from worker profile (name, location, language, etc.) and you can find part of their code (in Javascript) on [gustavotr/upwork-scraper](https://github.com/gustavotr/upwork-scraper). 

## Profile Link:
- name of worker
- link to profile page
- skill tags
- deliverable tags
\pic here

## Profile Data:

In short, I divide profile data to personal info, experience, task info and task info (optional). Please output n/a if the section or the info is **not available** in the worker's profile. 

1. Personal info (top & left banner as labeled in Figure 1):
	- profile page link

	- name of the worker
	
	- location of the worker (city, state and country)
	
	- job success rate
	
	- whether top-rated or not
	
	- occupation
	
	- ask price
	
	- personal description
	
	- total earning
	
	- total jobs
	
	- total hours
	
	- availability (< 30 hrs or > 30 hrs or upon request?)
	
	- languages (language name and proficiency)
	
	- verifications
	
	- education (institution name, program name, start & end years)
	
	- intermediary affiliation (name, hours, job success rate
	![personal_info_example](https://github.com/ruizuo11/geoWageGap/blob/main/personal_info_example.png?raw=true)

2. Experience (Figure 2):

  - skills tags 

  - certificate tags

  - employer name, start & end time of employment
![experience_example](https://github.com/ruizuo11/geoWageGap/blob/main/experience_example.png?raw=true) 

3. Task info (right banner as labeled in Figure 3):
	- no. completed jobs, no. processing jobs
	
	- task name
	
	- start & end date od task
	
	- earnings (if hourly earning then hrly price, hrs, and total earnings; if fixed price then total earnings; if private earning then output n/a)
	
	- client's rating &  comment
	
	- task description (output n/a if private task)
	

![task_info1_example](https://github.com/ruizuo11/geoWageGap/blob/main/task_info1_example.png?raw=true)
	
4. Task info labeled in Figure 4 is **optional**
	
	- skills required (output n/a if private task)
	
	- level of expertise required (output n/a if private task)
	
	- client's location, total spending & experience (output n/a if private task)
	

![task_info2_example](https://github.com/ruizuo11/geoWageGap/blob/main/task_info2_example.png?raw=true)
	



