## Problems in the UpWork Scraper

### Some meta-questions

- How do you debug without getting flagged by the website? I tried to debug the url scrapper, but then UpWork warned my account for frequent login. 
- How do you view the structure of the true (decoded) Javascript code that contains the worker info?
- Does rotating IP on server makes the account vulnerable because of changing IP address? 

### primary change, "recent task section":

- "start end date": the current result only includes the start date but not **end date**
- "start end date": start date is highly repetitive and does **not** align with reality 

![start_end_date](C:\Users\ruizu\mydoc\gig economy\upwork_scrape\start_end_date.png)

- "total earning": highly repetitive earning that does **not** align with reality

  ![total_earning](C:\Users\ruizu\mydoc\gig economy\upwork_scrape\total_earning.png)

- 'client location': recursively adds the location in previous task and does **not** align with the reality

  ![client_loc](C:\Users\ruizu\mydoc\gig economy\upwork_scrape\client_loc.png)

- Generally, **every** variable in "recent task" section is problematic and bears the same problem

### secondary change:

- "job success rate" not "job sucess rate"![job_success_rate](C:\Users\ruizu\mydoc\gig economy\upwork_scrape\job_success_rate.png)

- language returns strings not dictionary![languange](C:\Users\ruizu\mydoc\gig economy\upwork_scrape\languange.png)

- education returns repeated results (for every education experience, the result repeats once)

  ![education](C:\Users\ruizu\mydoc\gig economy\upwork_scrape\education.png)



