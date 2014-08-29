To schedule running of the script that rebuilds the models every 5 minutes run:
```
crontab -e
```

and add the following

```
*/5 * * * * cd "/SHINY_PATH/retpred_shiny/retdb_admin/scheduled_tasks" && Rscript "/SHINY_PATH/retpred_shiny/retdb_admin/scheduled_tasks/calc_all_models.R"
```
replacing SHINY_PATH appropriately.