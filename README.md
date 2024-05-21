# IOS_Personal
This repo is used only for learning Swift and building IOS applications


# How To Execute
​
## PATH 1
​
### Set Environment Variables:
​
- `TASK = DELINK_PMV`
- `LOADCSV = FALSE` (To fetch from DB)
- `MODE = LIMIT` (To update limited accounts in DB)
- `LIMIT = n` (n = desired number of records to be updated)
​
## PATH 2
​
### Set Environment Variables:
​
- `TASK = DELINK_PMV`
- `LOADCSV = false` (To fetch from DB)
- `MODE = ALL` (To update all records in DB)
​
## PATH 3
​
1. Update `all_pmv_ctplb_active_banks.csv` and add the records of `cust_to_plaid_linked_bank_id` and `plaid_access_token` of the desired users.
2. Set Environment Variables:
​
- `TASK = DELINK_PMV`
- `LOADCSV = true` (To fetch from CSV)
​
## In Case of FAILURE
​
- If it fails to delink, user details will be printed in the console.
- If it fails to update the DB, the update query will be generated in `pending_db_update_query.sql`.