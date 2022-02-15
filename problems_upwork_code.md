## Problems in the UpWork Scraper

### Some meta-questions

- How do you debug without getting flagged by the website? I tried to debug the url scrapper, but then UpWork warned my account for frequent login. 
- How do you view the structure of the true (decoded) Javascript code that contains the worker info?
- Does rotating IP on server makes the account vulnerable because of changing IP address? 

### primary change, "recent task section":

- "start end date": the current result only includes the start date but not **end date**
- "start end date": start date is highly repetitive and does **not** align with reality 

![start_end_date](https://github.com/ruizuo11/geoWageGap/blob/main/figures/start_end_date.png?raw=true)

- "total earning": highly repetitive earning that does **not** align with reality

  ![total_earning](https://github.com/ruizuo11/geoWageGap/blob/main/figures/total_earning.png?raw=true)

- 'client location': recursively adds the location in previous task and does **not** align with the reality

  ![client_loc](https://github.com/ruizuo11/geoWageGap/blob/main/figures/client_loc.png?raw=true)

- Generally, **every** variable in "recent task" section is problematic and bears the same problem

### secondary change:

- "job success rate" not "job sucess rate"![job_success_rate](https://github.com/ruizuo11/geoWageGap/blob/main/figures/figures/job_success_rate.png?raw=true)

- language returns strings not dictionary![languange](https://github.com/ruizuo11/geoWageGap/blob/main/languange.png?raw=true)

- education returns repeated results (for every education experience, the result repeats once)

  ![education](https://github.com/ruizuo11/geoWageGap/blob/main/figures/education.png?raw=true)



