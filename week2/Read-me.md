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

```
