# Week2 assignment

### Question 1. Load January 2020 data

q1: How many rows does that dataset have?

ans: 447,770

```
22:48:25.121 | INFO    | Task run 'clean-b9fd7e03-0' - rows: 447770
22:48:25.143 | INFO    | Task run 'clean-b9fd7e03-0' - Finished in state Completed()
```
### Question 2. Scheduling with Cron

q2:Using the flow in etl_web_to_gcs.py, create a deployment to run on the first of every month at 5am UTC. What’s the cron schedule for that?

ans: 0 5 1 * *


![Screenshot from 2023-02-06 16-33-29](https://user-images.githubusercontent.com/48046561/216955603-4eb9b832-980b-4435-81c7-ecc48f4b34f2.png)

### Question 3 .Loading data to BigQuery [script for this](https://github.com/Dinakaranevil/Data-engineering-HW-/blob/main/week2/parameterised_etl_gcs_to_bq.py) 


ans :14,851,920


![Screenshot from 2023-02-06 14-16-10](https://user-images.githubusercontent.com/48046561/216956637-d85ac56e-4d88-4ce9-85f0-dc195b376778.png)

### Question 4 Github Storage Block[script for this](https://github.com/Dinakaranevil/Data-engineering-HW-/blob/main/week2/github.py)

ans :88605

![Screenshot from 2023-02-06 16-45-35](https://user-images.githubusercontent.com/48046561/216957998-cf1f3382-9db2-4fbe-98f6-31966a261f87.png)


### Question 5 
Run: prefect cloud login -k MY_PREFECT_API_KEY 
     prefect block register -m prefect_gcp 
     prefect deployment build flows/etl_web_to_gcs.py:etl_parent_flow -n cloud_flow_deployment -sb github/git --apply 
     prefect agent start --work-queue "default" 

ans : 514392


### Question 6 Secrets
![Screenshot from 2023-02-06 16-48-22](https://user-images.githubusercontent.com/48046561/216958434-545743d6-36a7-46c1-9e3a-d362bf359601.png)
ans : 8




